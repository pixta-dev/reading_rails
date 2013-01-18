# 第一回
- `which rails` >> /Users/Altech/.rvm/gems/ruby-1.9.3-p286/bin/rails
- `load Gem.bin_path('railties', 'rails', version)` >> gem(railties)/bin/rails
- `require "rails/cli"` >> gem(railties)/lib/rails/cli.rb
- `require 'rails/script_rails_loader'; Rails::ScriptRailsLoader.exec_script_rails!` >> (app)/script/rails
  - ここでプロセスが(app)/script/railsに変身
  - (app)/script/railsの`require File.expand_path('../../config/boot',  __FILE__)`でBundlerチェックなど
- `require 'rails/commands'` >> gem(railties)/lib/rails/commands.rb
  - ここで引数処理. 今回は引数serverの場合を追う.
- `require 'rails/commands/server'` >> gem(railties)/lib/rails/commands/server.rb
  - `server.rb`の冒頭で`require 'action_dispatch'`。ActionPackのもの。action_dispatchでRackをrequireしている。
  - `Rails::Server << Rack::Server`
- `Rails::Server.new.tap{ ...  }` >> commands.rbに戻ってきて、tapの中身
- `require APP_PATH` >> (app)/config/application.rb
  - `rails/all`して各種Railsコンポーネント読み込み
  - `Bundler.require(*Rails.groups(:assets => %w(development test)))`でGemfileのrequire
  - `SampleApp::Application < Rails::Application`を定義
- `server.start` >> gem(railties)/lib/rails/commands/server.rb # tapに戻って
- `super` >> gem(rack)/lib/rack/server.rb # インスタンスメソッドの方
- `wrapped_app` >> `app`
  - appメソッドでconfig.ruの読み込み、Rails::Applicationを返す
  - `build_app`で、appから返ってきたRails::Applicationを薄くラッピング）
- `server.run wrapped_app, options, &blk`でサーバー起動！

ここまででサーバー起動したのでそこから。

    def server
      @_server ||= Rack::Handler.get(options[:server]) || Rack::Handler.default(options)
    end

