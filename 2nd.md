# 第二回

## 参考資料
- [第23回　Rackとは何か（1）Rackの生まれた背景：Ruby Freaks Lounge｜gihyo.jp … 技術評論社](http://gihyo.jp/dev/serial/01/ruby/0023)
  - `config.ru`のruは`rackup`
- [ちょっとわかるrack - SSSSLIDE](http://sssslide.com/speakerdeck.com/lchin/rack)

## メモ
["/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/pry_instance.rb:275:in `eval'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/pry_instance.rb:275:in `re'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/pry_instance.rb:251:in `rep'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/pry_instance.rb:231:in `block (3 levels) in repl'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/pry_instance.rb:230:in `loop'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/pry_instance.rb:230:in `block (2 levels) in repl'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/pry_instance.rb:229:in `catch'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/pry_instance.rb:229:in `block in repl'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/pry_instance.rb:228:in `catch'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/pry_instance.rb:228:in `repl'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/pry_class.rb:154:in `start'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/pry-0.9.10/lib/pry/core_extensions.rb:22:in `pry'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railties/controller_runtime.rb:17:in `process_action'",  # ここまでがcontroller内の処理
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/abstract_controller/base.rb:121:in `process'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/abstract_controller/rendering.rb:45:in `process'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/metal.rb:203:in `dispatch'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/metal/rack_delegation.rb:14:in `dispatch'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/metal.rb:246:in `block in action'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/routing/route_set.rb:73:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/routing/route_set.rb:73:in `dispatch'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/routing/route_set.rb:36:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/journey-1.0.4/lib/journey/router.rb:68:in `block in call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/journey-1.0.4/lib/journey/router.rb:56:in `each'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/journey-1.0.4/lib/journey/router.rb:56:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/routing/route_set.rb:601:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/best_standards_support.rb:17:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/rack-1.4.4/lib/rack/etag.rb:23:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/rack-1.4.4/lib/rack/conditionalget.rb:25:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/head.rb:14:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/params_parser.rb:21:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/flash.rb:242:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/rack-1.4.4/lib/rack/session/abstract/id.rb:210:in `context'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/rack-1.4.4/lib/rack/session/abstract/id.rb:205:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/cookies.rb:341:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/query_cache.rb:64:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/connection_adapters/abstract/connection_pool.rb:479:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/callbacks.rb:28:in `block in call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/callbacks.rb:405:in `_run__2816320416663906372__call__2680822319256969416__callbacks'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/callbacks.rb:405:in `__run_callback'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/callbacks.rb:385:in `_run_call_callbacks'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/callbacks.rb:81:in `run_callbacks'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/callbacks.rb:27:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/reloader.rb:65:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/remote_ip.rb:31:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/debug_exceptions.rb:16:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/show_exceptions.rb:56:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/rack/logger.rb:32:in `call_app'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/rack/logger.rb:16:in `block in call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/tagged_logging.rb:22:in `tagged'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/rack/logger.rb:16:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/request_id.rb:22:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/rack-1.4.4/lib/rack/methodoverride.rb:21:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/rack-1.4.4/lib/rack/runtime.rb:17:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/cache/strategy/local_cache.rb:72:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/rack-1.4.4/lib/rack/lock.rb:15:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/middleware/static.rb:62:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:479:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/application.rb:223:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/rack-1.4.4/lib/rack/content_length.rb:14:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/rack/log_tailer.rb:17:in `call'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/rack-1.4.4/lib/rack/handler/webrick.rb:59:in `service'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/1.9.1/webrick/httpserver.rb:138:in `service'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/1.9.1/webrick/httpserver.rb:94:in `run'",
 "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/1.9.1/webrick/server.rb:191:in `block in start_thread'"]

- rack-1.4.4/lib/rackにpry
  - @appの中身
#<SampleApp::Application:0x007ff8c3a19708
 @_all_autoload_paths=
  ["/Users/Altech/dev/reading/sample_app/app/assets",
   "/Users/Altech/dev/reading/sample_app/app/controller",
   "/Users/Altech/dev/reading/sample_app/app/controllers",
   "/Users/Altech/dev/reading/sample_app/app/helpers",
   "/Users/Altech/dev/reading/sample_app/app/mailers",
   "/Users/Altech/dev/reading/sample_app/app/models"],
 @_all_load_paths=
  ["/Users/Altech/dev/reading/sample_app/lib",
   "/Users/Altech/dev/reading/sample_app/vendor",
   "/Users/Altech/dev/reading/sample_app/app/assets",
   "/Users/Altech/dev/reading/sample_app/app/controller",
   "/Users/Altech/dev/reading/sample_app/app/controllers",
   "/Users/Altech/dev/reading/sample_app/app/helpers",
   "/Users/Altech/dev/reading/sample_app/app/mailers",
   "/Users/Altech/dev/reading/sample_app/app/models"],
 @app=
  #<ActionDispatch::Static:0x007ff8c643f7a8
   @app=
    #<Rack::Lock:0x007ff8c6423c88
     @app=
      #<ActiveSupport::Cache::Strategy::LocalCache::Middleware:0x007ff8c36951b8
       @app=
        #<Rack::Runtime:0x007ff8c6423d28
         @app=
          #<Rack::MethodOverride:0x007ff8c6423d50
           @app=
            #<ActionDispatch::RequestId:0x007ff8c6423dc8
             @app=
              #<Rails::Rack::Logger:0x007ff8c6423e40
               @app=
                #<ActionDispatch::ShowExceptions:0x007ff8c6423eb8
                 @app=
                  #<ActionDispatch::DebugExceptions:0x007ff8c6423f08
                   @app=
                    #<ActionDispatch::RemoteIp:0x007ff8c6423f58
                     @app=
                      #<ActionDispatch::Reloader:0x007ff8c6423f80
                       @app=
                        #<ActionDispatch::Callbacks:0x007ff8c6423fa8
                         @app=
                          #<ActiveRecord::ConnectionAdapters::ConnectionManagement:0x007ff8c6423ff8
                           @app=
                            #<ActiveRecord::QueryCache:0x007ff8c620c8a0
                             @app=
                              #<ActionDispatch::Cookies:0x007ff8c634c3c8
                               @app=
                                #<ActionDispatch::Session::CookieStore:0x007ff8c634ca08
                                 @app=
                                  #<ActionDispatch::Flash:0x007ff8c634cb20
                                   @app=
                                    #<ActionDispatch::ParamsParser:0x007ff8c634cda0
                                     @app=
                                      #<ActionDispatch::Head:0x007ff8c634cdc8
                                       @app=
                                        #<Rack::ConditionalGet:0x007ff8c634cf08
                                         @app=
                                          #<Rack::ETag:0x007ff8c634cf58
                                           @app=
                                            #<ActionDispatch::BestStandardsSupport:0x007ff8c634d0c0
                                             @app=
                                              #<ActionDispatch::Routing::RouteSet:0x007ff8c62aa320>,
                                             @header="IE=Edge">,
                                           @cache_control=
                                            "max-age=0, private, must-revalidate",
                                           @no_cache_control="no-cache">>>,
                                     @parsers=
                                      {application/xml=>:xml_simple,
                                       application/json=>:json}>>,
                                 @coder=
                                  #<Rack::Session::Cookie::Base64::Marshal:0x007ff8c634c4e0>,
                                 @cookie_only=true,
                                 @default_options=
                                  {:path=>"/",
                                   :domain=>nil,
                                   :expire_after=>nil,
                                   :secure=>false,
                                   :httponly=>true,
                                   :defer=>false,
                                   :renew=>false,
                                   :secret=>
                                    "7dc802f779c58d5b6f87c123f0ab78b12fdda4a56bb33c8f03d4bfdee551",
                                   :coder=>
                                    #<Rack::Session::Cookie::Base64::Marshal:0x007ff8c634c4e0>},
                                 @key="_sample_app_session",
                                 @secrets=
                                  ["7dc802f779c58d5b6f87c123f0ab78b12fdda4a56bb33c8f03d4bfdee551"]>>>>>,
                       @condition=
                        #<Proc:0x007ff8c6129578@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/application.rb:267 (lambda)>,
                       @validated=true>,
                     @check_ip=true,
                     @proxies=
                      /
      ^127\.0\.0\.1$                | # localhost
      ^(10                          | # private IP 10.x.x.x
        172\.(1[6-9]|2[0-9]|3[0-1]) | # private IP in the range 172.16.0.0 .. 172.31.255.255
        192\.168                      # private IP 192.168.x.x
       )\.
    /x>>,
                 @exceptions_app=
                  #<ActionDispatch::PublicExceptions:0x007ff8c633c6a8
                   @public_path=
                    "/Users/Altech/dev/reading/sample_app/public">>,
               @taggers=[]>>>,
         @header_name="X-Runtime">,
       @name="ActiveSupport::Cache::Strategy::LocalCache",
       @thread_local_key=
        :active_support_cache_file_store_local_cache_70353226378980>,
     @mutex=#<Mutex:0x007ff8c6423c60>>,
   @file_handler=
    #<ActionDispatch::FileHandler:0x007ff8c643f758
     @compiled_root=/^\/Users\/Altech\/dev\/reading\/sample_app\/public/,
     @file_server=
      #<Rack::File:0x007ff8c3cdfbb8
       @headers=nil,
       @root="/Users/Altech/dev/reading/sample_app/public">,
     @root="/Users/Altech/dev/reading/sample_app/public">>,
 @assets=
  #<Sprockets::Environment:0x3ffc61b8f7d4 root="/Users/Altech/dev/reading/sample_app", paths=["/Users/Altech/dev/reading/sample_app/app/assets/images", "/Users/Altech/dev/reading/sample_app/app/assets/javascripts", "/Users/Altech/dev/reading/sample_app/app/assets/stylesheets", "/Users/Altech/dev/reading/sample_app/vendor/assets/javascripts", "/Users/Altech/dev/reading/sample_app/vendor/assets/stylesheets", "/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/jquery-rails-2.1.4/vendor/assets/javascripts", "/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/coffee-rails-3.2.2/lib/assets/javascripts"], digest="6776f581a4329e299531e1d52aa59832">,
 @config=
  #<Rails::Application::Configuration:0x007ff8c3b11110
   @allow_concurrency=false,
   @assets=
    {:enabled=>true,
     :paths=>
      ["/Users/Altech/dev/reading/sample_app/app/assets/images",
       "/Users/Altech/dev/reading/sample_app/app/assets/javascripts",
       "/Users/Altech/dev/reading/sample_app/app/assets/stylesheets",
       "/Users/Altech/dev/reading/sample_app/vendor/assets/javascripts",
       "/Users/Altech/dev/reading/sample_app/vendor/assets/stylesheets",
       "/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/jquery-rails-2.1.4/vendor/assets/javascripts",
       "/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/coffee-rails-3.2.2/lib/assets/javascripts"],
     :precompile=>
      [#<Proc:0x007ff8c3b0eaa0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/application/configuration.rb:48>,
       /(?:\/|\\|\A)application\.(css|js)$/],
     :prefix=>"/assets",
     :version=>"1.0",
     :debug=>true,
     :compile=>true,
     :digest=>false,
     :manifest=>nil,
     :cache_store=>
      [:file_store, "/Users/Altech/dev/reading/sample_app/tmp/cache/assets/"],
     :js_compressor=>nil,
     :css_compressor=>nil,
     :initialize_on_precompile=>true,
     :logger=>nil,
     :compress=>false},
   @autoload_once_paths=[],
   @autoload_paths=[],
   @cache_classes=false,
   @cache_store=
    [:file_store, "/Users/Altech/dev/reading/sample_app/tmp/cache/"],
   @consider_all_requests_local=true,
   @dependency_loading=true,
   @eager_load_paths=
    ["/Users/Altech/dev/reading/sample_app/app/assets",
     "/Users/Altech/dev/reading/sample_app/app/controller",
     "/Users/Altech/dev/reading/sample_app/app/controllers",
     "/Users/Altech/dev/reading/sample_app/app/helpers",
     "/Users/Altech/dev/reading/sample_app/app/mailers",
     "/Users/Altech/dev/reading/sample_app/app/models"],
   @encoding="utf-8",
   @exceptions_app=nil,
   @file_watcher=ActiveSupport::FileUpdateChecker,
   @filter_parameters=[:password],
   @force_ssl=false,
   @generators=
    #<Rails::Configuration::Generators:0x007ff8c3696658
     @aliases={},
     @colorize_logging=true,
     @fallbacks={},
     @hidden_namespaces=["sass"],
     @options=
      {:rails=>
        {:orm=>:active_record,
         :test_framework=>:test_unit,
         :integration_tool=>:test_unit,
         :performance_tool=>:test_unit,
         :stylesheet_engine=>:scss,
         :javascript_engine=>:coffee},
       :active_record=>{:migration=>true, :timestamps=>true},
       :test_unit=>{:fixture=>true, :fixture_replacement=>nil}},
     @templates=[]>,
   @helpers_paths=["/Users/Altech/dev/reading/sample_app/app/helpers"],
   @log_level=:debug,
   @middleware=
    #<ActionDispatch::MiddlewareStack:0x007ff8c377c8d8
     @middlewares=
      [ActionDispatch::Static,
       Rack::Lock,
       #<ActiveSupport::Cache::Strategy::LocalCache::Middleware:0x007ff8c36951b8>,
       Rack::Runtime,
       Rack::MethodOverride,
       ActionDispatch::RequestId,
       Rails::Rack::Logger,
       ActionDispatch::ShowExceptions,
       ActionDispatch::DebugExceptions,
       ActionDispatch::RemoteIp,
       ActionDispatch::Reloader,
       ActionDispatch::Callbacks,
       ActiveRecord::ConnectionAdapters::ConnectionManagement,
       ActiveRecord::QueryCache,
       ActionDispatch::Cookies,
       ActionDispatch::Session::CookieStore,
       ActionDispatch::Flash,
       ActionDispatch::ParamsParser,
       ActionDispatch::Head,
       Rack::ConditionalGet,
       Rack::ETag,
       ActionDispatch::BestStandardsSupport]>,
   @paths=
    {"app"=>["app"],
     "app/assets"=>["app/assets"],
     "app/controllers"=>["app/controllers"],
     "app/helpers"=>["app/helpers"],
     "app/models"=>["app/models"],
     "app/mailers"=>["app/mailers"],
     "app/views"=>["app/views"],
     "lib"=>["lib"],
     "lib/assets"=>["lib/assets"],
     "lib/tasks"=>["lib/tasks"],
     "config"=>["config"],
     "config/environments"=>["config/environments"],
     "config/initializers"=>["config/initializers"],
     "config/locales"=>["config/locales"],
     "config/routes"=>["config/routes.rb"],
     "db"=>["db"],
     "db/migrate"=>["db/migrate"],
     "db/seeds"=>["db/seeds.rb"],
     "vendor"=>["vendor"],
     "vendor/assets"=>["vendor/assets"],
     "vendor/plugins"=>["vendor/plugins"],
     "config/database"=>["config/database.yml"],
     "config/environment"=>["config/environment.rb"],
     "lib/templates"=>["lib/templates"],
     "log"=>["log/development.log"],
     "public"=>["public"],
     "public/javascripts"=>["public/javascripts"],
     "public/stylesheets"=>["public/stylesheets"],
     "tmp"=>["tmp"]},
   @railties_order=[:all],
   @relative_url_root=nil,
   @reload_classes_only_on_change=true,
   @root=#<Pathname:/Users/Altech/dev/reading/sample_app>,
   @secret_token=
    "71b16ed4a690561f778ebb488e51588a561d7bbcff10f98b1e7d641cff8724fa79f9047581c67890e67550a2bd180fd8bb295f9351430ac2577f874f7fc1891b",
   @serve_static_assets=true,
   @session_options=
    {:key=>"_sample_app_session",
     :secret=>"7dc802f779c58d5b6f87c123f0ab78b12fdda4a56bb33c8f03d4bfdee551",
     :coder=>#<Rack::Session::Cookie::Base64::Marshal:0x007ff8c634c4e0>,
     :cookie_only=>true},
   @session_store=:cookie_store,
   @ssl_options={},
   @static_cache_control=nil,
   @time_zone="UTC",
   @whiny_nils=true>,
 @initialized=true,
 @initializers=
  [#<Rails::Initializable::Initializer:0x007ff8c61d2ad8
    @block=
     #<Proc:0x007ff8c3a0a2a8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:524>,
    @context=#<SampleApp::Application:0x007ff8c3a19708 ...>,
    @name=:set_load_path,
    @options={:before=>:bootstrap_hook, :group=>:default}>,
   #<Rails::Initializable::Initializer:0x007ff8c61d2a88
    @block=
     #<Proc:0x007ff8c3a0a118@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:536>,
    @context=#<SampleApp::Application:0x007ff8c3a19708 ...>,
    @name=:set_autoload_paths,
    @options=
     {:before=>:bootstrap_hook, :after=>:set_load_path, :group=>:default}>,
   #<Rails::Initializable::Initializer:0x007ff8c61d2a10
    @block=
     #<Proc:0x007ff8c3a09f38@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:546>,
    @context=#<SampleApp::Application:0x007ff8c3a19708 ...>,
    @name=:add_routing_paths,
    @options={:after=>:set_autoload_paths, :group=>:default}>,
   #<Rails::Initializable::Initializer:0x007ff8c61d29c0
    @block=
     #<Proc:0x007ff8c3a09da8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:557>,
    @context=#<SampleApp::Application:0x007ff8c3a19708 ...>,
    @name=:add_locales,
    @options={:after=>:add_routing_paths, :group=>:default}>,
   #<Rails::Initializable::Initializer:0x007ff8c61d2948
    @block=
     #<Proc:0x007ff8c3a09bc8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:561>,
    @context=#<SampleApp::Application:0x007ff8c3a19708 ...>,
    @name=:add_view_paths,
    @options={:after=>:add_locales, :group=>:default}>,
   #<Rails::Initializable::Initializer:0x007ff8c61d28f8
    @block=
     #<Proc:0x007ff8c3a099e8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:569>,
    @context=#<SampleApp::Application:0x007ff8c3a19708 ...>,
    @name=:load_environment_config,
    @options=
     {:before=>:load_environment_hook, :group=>:all, :after=>:add_view_paths}>,
   #<Rails::Initializable::Initializer:0x007ff8c61d2880
    @block=
     #<Proc:0x007ff8c3a09858@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:574>,
    @context=#<SampleApp::Application:0x007ff8c3a19708 ...>,
    @name=:append_assets_path,
    @options={:group=>:all, :after=>:load_environment_config}>,
   #<Rails::Initializable::Initializer:0x007ff8c61d2830
    @block=
     #<Proc:0x007ff8c3a09678@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:580>,
    @context=#<SampleApp::Application:0x007ff8c3a19708 ...>,
    @name=:prepend_helpers_path,
    @options={:after=>:append_assets_path, :group=>:default}>,
   #<Rails::Initializable::Initializer:0x007ff8c61d27b8
    @block=
     #<Proc:0x007ff8c3a093f8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:586>,
    @context=#<SampleApp::Application:0x007ff8c3a19708 ...>,
    @name=:load_config_initializers,
    @options={:after=>:prepend_helpers_path, :group=>:default}>,
   #<Rails::Initializable::Initializer:0x007ff8c61d2768
    @block=
     #<Proc:0x007ff8c3a09218@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:592>,
    @context=#<SampleApp::Application:0x007ff8c3a19708 ...>,
    @name=:engines_blank_point,
    @options={:after=>:load_config_initializers, :group=>:default}>],
 @ordered_railties=
  [#<I18n::Railtie:0x007ff8c6070500
    @config=#<Rails::Railtie::Configuration:0x007ff8c60c1720>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c614c550
       @block=
        #<Proc:0x007ff8c60c0f50@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/i18n_railtie.rb:24>,
       @context=#<I18n::Railtie:0x007ff8c6070500 ...>,
       @name="i18n.callbacks",
       @options={:group=>:default}>]>,
   #<ActiveSupport::Railtie:0x007ff8c60c0a50
    @config=#<Rails::Railtie::Configuration:0x007ff8c60c0a28>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c614c230
       @block=
        #<Proc:0x007ff8c60c0848@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/railtie.rb:10>,
       @context=#<ActiveSupport::Railtie:0x007ff8c60c0a50 ...>,
       @name="active_support.initialize_whiny_nils",
       @options={:group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c614c1e0
       @block=
        #<Proc:0x007ff8c60c0758@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/railtie.rb:14>,
       @context=#<ActiveSupport::Railtie:0x007ff8c60c0a50 ...>,
       @name="active_support.deprecation_behavior",
       @options=
        {:after=>"active_support.initialize_whiny_nils", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c614c168
       @block=
        #<Proc:0x007ff8c60c0668@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/railtie.rb:46>,
       @context=#<ActiveSupport::Railtie:0x007ff8c60c0a50 ...>,
       @name="active_support.initialize_time_zone",
       @options=
        {:after=>"active_support.deprecation_behavior", :group=>:default}>]>,
   #<ActionDispatch::Railtie:0x007ff8c610c770
    @config=#<Rails::Railtie::Configuration:0x007ff8c610c748>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c614be48
       @block=
        #<Proc:0x007ff8c61281c8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/railtie.rb:22>,
       @context=#<ActionDispatch::Railtie:0x007ff8c610c770 ...>,
       @name="action_dispatch.configure",
       @options={:group=>:default}>]>,
   #<ActionView::Railtie:0x007ff8c3760b10
    @config=#<Rails::Railtie::Configuration:0x007ff8c3760ae8>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c614bab0
       @block=
        #<Proc:0x007ff8c37602c8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_view/railtie.rb:12>,
       @context=#<ActionView::Railtie:0x007ff8c3760b10 ...>,
       @name="action_view.embed_authenticity_token_in_remote_forms",
       @options={:group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c614ba38
       @block=
        #<Proc:0x007ff8c3760160@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_view/railtie.rb:19>,
       @context=#<ActionView::Railtie:0x007ff8c3760b10 ...>,
       @name="action_view.cache_asset_ids",
       @options=
        {:after=>"action_view.embed_authenticity_token_in_remote_forms",
         :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c614b9e8
       @block=
        #<Proc:0x007ff8c375fff8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_view/railtie.rb:27>,
       @context=#<ActionView::Railtie:0x007ff8c3760b10 ...>,
       @name="action_view.javascript_expansions",
       @options={:after=>"action_view.cache_asset_ids", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c614b970
       @block=
        #<Proc:0x007ff8c375feb8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_view/railtie.rb:39>,
       @context=#<ActionView::Railtie:0x007ff8c3760b10 ...>,
       @name="action_view.set_configs",
       @options=
        {:after=>"action_view.javascript_expansions", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c614b920
       @block=
        #<Proc:0x007ff8c375fdc8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_view/railtie.rb:47>,
       @context=#<ActionView::Railtie:0x007ff8c3760b10 ...>,
       @name="action_view.caching",
       @options={:after=>"action_view.set_configs", :group=>:default}>]>,
   #<ActionController::Railtie:0x007ff8c3697328
    @config=#<Rails::Railtie::Configuration:0x007ff8c3697300>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c614b560
       @block=
        #<Proc:0x007ff8c3697030@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/railtie.rb:12>,
       @context=#<ActionController::Railtie:0x007ff8c3697328 ...>,
       @name="action_controller.logger",
       @options={:group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c614b4e8
       @block=
        #<Proc:0x007ff8c3696ef0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/railtie.rb:16>,
       @context=#<ActionController::Railtie:0x007ff8c3697328 ...>,
       @name="action_controller.initialize_framework_caches",
       @options={:after=>"action_controller.logger", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c614b498
       @block=
        #<Proc:0x007ff8c3696d88@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/railtie.rb:20>,
       @context=#<ActionController::Railtie:0x007ff8c3697328 ...>,
       @name="action_controller.assets_config",
       @options=
        {:group=>:all,
         :after=>"action_controller.initialize_framework_caches"}>,
      #<Rails::Initializable::Initializer:0x007ff8c614b420
       @block=
        #<Proc:0x007ff8c3696cc0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/railtie.rb:24>,
       @context=#<ActionController::Railtie:0x007ff8c3697328 ...>,
       @name="action_controller.set_configs",
       @options={:after=>"action_controller.assets_config", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c61533a0
       @block=
        #<Proc:0x007ff8c3696ba8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/railtie.rb:45>,
       @context=#<ActionController::Railtie:0x007ff8c3697328 ...>,
       @name="action_controller.compile_config_methods",
       @options={:after=>"action_controller.set_configs", :group=>:default}>]>,
   #<ActiveRecord::Railtie:0x007ff8c3696838
    @config=#<Rails::Railtie::Configuration:0x007ff8c3696810>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c6152fb8
       @block=
        #<Proc:0x007ff8c3695e88@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:44>,
       @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
       @name="active_record.initialize_timezone",
       @options={:group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6152f68
       @block=
        #<Proc:0x007ff8c3695d48@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:51>,
       @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
       @name="active_record.logger",
       @options=
        {:after=>"active_record.initialize_timezone", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6152ef0
       @block=
        #<Proc:0x007ff8c3695c58@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:55>,
       @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
       @name="active_record.identity_map",
       @options={:after=>"active_record.logger", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6152ea0
       @block=
        #<Proc:0x007ff8c3695b40@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:60>,
       @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
       @name="active_record.set_configs",
       @options={:after=>"active_record.identity_map", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6152e28
       @block=
        #<Proc:0x007ff8c3695a28@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:73>,
       @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
       @name="active_record.initialize_database",
       @options={:after=>"active_record.set_configs", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6152dd8
       @block=
        #<Proc:0x007ff8c3695938@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:87>,
       @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
       @name="active_record.log_runtime",
       @options=
        {:after=>"active_record.initialize_database", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6152d60
       @block=
        #<Proc:0x007ff8c3695820@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:94>,
       @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
       @name="active_record.set_reloader_hooks",
       @options={:after=>"active_record.log_runtime", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6152ce8
       @block=
        #<Proc:0x007ff8c3695708@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:111>,
       @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
       @name="active_record.add_watchable_files",
       @options=
        {:after=>"active_record.set_reloader_hooks", :group=>:default}>]>,
   #<ActionMailer::Railtie:0x007ff8c3045cb8
    @config=#<Rails::Railtie::Configuration:0x007ff8c3045c90>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c61529a0
       @block=
        #<Proc:0x007ff8c30445c0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionmailer-3.2.11/lib/action_mailer/railtie.rb:9>,
       @context=#<ActionMailer::Railtie:0x007ff8c3045cb8 ...>,
       @name="action_mailer.logger",
       @options={:group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6152928
       @block=
        #<Proc:0x007ff8c3043760@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionmailer-3.2.11/lib/action_mailer/railtie.rb:13>,
       @context=#<ActionMailer::Railtie:0x007ff8c3045cb8 ...>,
       @name="action_mailer.set_configs",
       @options={:after=>"action_mailer.logger", :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c61528d8
       @block=
        #<Proc:0x007ff8c3046f50@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionmailer-3.2.11/lib/action_mailer/railtie.rb:38>,
       @context=#<ActionMailer::Railtie:0x007ff8c3045cb8 ...>,
       @name="action_mailer.compile_config_methods",
       @options={:after=>"action_mailer.set_configs", :group=>:default}>]>,
   #<ActiveResource::Railtie:0x007ff8c30c85a0
    @config=#<Rails::Railtie::Configuration:0x007ff8c30c8410>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c61525b8
       @block=
        #<Proc:0x007ff8c30ce5e0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activeresource-3.2.11/lib/active_resource/railtie.rb:8>,
       @context=#<ActiveResource::Railtie:0x007ff8c30c85a0 ...>,
       @name="active_resource.set_configs",
       @options={:group=>:default}>]>,
   #<Rails::TestUnitRailtie:0x007ff8c30e7d88
    @config=#<Rails::Railtie::Configuration:0x007ff8c30e7d60>,
    @initializers=[]>,
   #<Sprockets::Railtie:0x007ff8c317b7e0
    @config=#<Rails::Railtie::Configuration:0x007ff8c317b420>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c6151f78
       @block=
        #<Proc:0x007ff8c317bab0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/sprockets/railtie.rb:17>,
       @context=#<Sprockets::Railtie:0x007ff8c317b7e0 ...>,
       @name="sprockets.environment",
       @options={:group=>:all}>]>,
   #<Sass::Rails::Railtie:0x007ff8c37ac8d0
    @config=#<Rails::Railtie::Configuration:0x007ff8c37ac880>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c6151c58
       @block=
        #<Proc:0x007ff8c610c5b8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/sass-rails-3.2.6/lib/sass/rails/railtie.rb:47>,
       @context=#<Sass::Rails::Railtie:0x007ff8c37ac8d0 ...>,
       @name=:setup_sass,
       @options={:group=>:all}>,
      #<Rails::Initializable::Initializer:0x007ff8c6151be0
       @block=
        #<Proc:0x007ff8c610c4f0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/sass-rails-3.2.6/lib/sass/rails/railtie.rb:73>,
       @context=#<Sass::Rails::Railtie:0x007ff8c37ac8d0 ...>,
       @name=:setup_compression,
       @options={:group=>:all, :after=>:setup_sass}>]>,
   #<Jquery::Rails::Railtie:0x007ff8c31de3e0
    @config=#<Rails::Railtie::Configuration:0x007ff8c31de0e8>,
    @initializers=[]>,
   #<Coffee::Rails::Engine:0x007ff8c3d9b9a8
    @_all_autoload_paths=[],
    @_all_load_paths=
     ["/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/coffee-rails-3.2.2/lib"],
    @config=
     #<Rails::Engine::Configuration:0x007ff8c480eca0
      @autoload_once_paths=[],
      @autoload_paths=[],
      @eager_load_paths=[],
      @generators=
       #<Rails::Configuration::Generators:0x007ff8c480ec28
        @aliases={},
        @colorize_logging=true,
        @fallbacks={},
        @hidden_namespaces=["sass"],
        @options=
         {:rails=>
           {:orm=>:active_record,
            :test_framework=>:test_unit,
            :integration_tool=>:test_unit,
            :performance_tool=>:test_unit,
            :stylesheet_engine=>:scss},
          :active_record=>{:migration=>true, :timestamps=>true},
          :test_unit=>{:fixture=>true, :fixture_replacement=>nil}},
        @templates=[]>,
      @paths=
       {"app"=>["app"],
        "app/assets"=>["app/assets"],
        "app/controllers"=>["app/controllers"],
        "app/helpers"=>["app/helpers"],
        "app/models"=>["app/models"],
        "app/mailers"=>["app/mailers"],
        "app/views"=>["app/views"],
        "lib"=>["lib"],
        "lib/assets"=>["lib/assets"],
        "lib/tasks"=>["lib/tasks"],
        "config"=>["config"],
        "config/environments"=>["config/environments"],
        "config/initializers"=>["config/initializers"],
        "config/locales"=>["config/locales"],
        "config/routes"=>["config/routes.rb"],
        "db"=>["db"],
        "db/migrate"=>["db/migrate"],
        "db/seeds"=>["db/seeds.rb"],
        "vendor"=>["vendor"],
        "vendor/assets"=>["vendor/assets"],
        "vendor/plugins"=>["vendor/plugins"]},
      @root=
       #<Pathname:/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/coffee-rails-3.2.2>>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c61570b8
       @block=
        #<Proc:0x007ff8c3a0a2a8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:524>,
       @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
       @name=:set_load_path,
       @options={:before=>:bootstrap_hook, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6157040
       @block=
        #<Proc:0x007ff8c3a0a118@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:536>,
       @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
       @name=:set_autoload_paths,
       @options=
        {:before=>:bootstrap_hook, :after=>:set_load_path, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6156fc8
       @block=
        #<Proc:0x007ff8c3a09f38@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:546>,
       @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
       @name=:add_routing_paths,
       @options={:after=>:set_autoload_paths, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6156f78
       @block=
        #<Proc:0x007ff8c3a09da8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:557>,
       @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
       @name=:add_locales,
       @options={:after=>:add_routing_paths, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6156f00
       @block=
        #<Proc:0x007ff8c3a09bc8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:561>,
       @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
       @name=:add_view_paths,
       @options={:after=>:add_locales, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6156e88
       @block=
        #<Proc:0x007ff8c3a099e8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:569>,
       @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
       @name=:load_environment_config,
       @options=
        {:before=>:load_environment_hook,
         :group=>:all,
         :after=>:add_view_paths}>,
      #<Rails::Initializable::Initializer:0x007ff8c6156e38
       @block=
        #<Proc:0x007ff8c3a09858@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:574>,
       @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
       @name=:append_assets_path,
       @options={:group=>:all, :after=>:load_environment_config}>,
      #<Rails::Initializable::Initializer:0x007ff8c6156dc0
       @block=
        #<Proc:0x007ff8c3a09678@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:580>,
       @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
       @name=:prepend_helpers_path,
       @options={:after=>:append_assets_path, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6156d70
       @block=
        #<Proc:0x007ff8c3a093f8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:586>,
       @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
       @name=:load_config_initializers,
       @options={:after=>:prepend_helpers_path, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c6156cf8
       @block=
        #<Proc:0x007ff8c3a09218@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:592>,
       @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
       @name=:engines_blank_point,
       @options={:after=>:load_config_initializers, :group=>:default}>],
    @railties=
     #<Rails::Engine::Railties:0x007ff8c61517f8
      @all=[],
      @config=
       #<Rails::Engine::Configuration:0x007ff8c480eca0
        @autoload_once_paths=[],
        @autoload_paths=[],
        @eager_load_paths=[],
        @generators=
         #<Rails::Configuration::Generators:0x007ff8c480ec28
          @aliases={},
          @colorize_logging=true,
          @fallbacks={},
          @hidden_namespaces=["sass"],
          @options=
           {:rails=>
             {:orm=>:active_record,
              :test_framework=>:test_unit,
              :integration_tool=>:test_unit,
              :performance_tool=>:test_unit,
              :stylesheet_engine=>:scss},
            :active_record=>{:migration=>true, :timestamps=>true},
            :test_unit=>{:fixture=>true, :fixture_replacement=>nil}},
          @templates=[]>,
        @paths=
         {"app"=>["app"],
          "app/assets"=>["app/assets"],
          "app/controllers"=>["app/controllers"],
          "app/helpers"=>["app/helpers"],
          "app/models"=>["app/models"],
          "app/mailers"=>["app/mailers"],
          "app/views"=>["app/views"],
          "lib"=>["lib"],
          "lib/assets"=>["lib/assets"],
          "lib/tasks"=>["lib/tasks"],
          "config"=>["config"],
          "config/environments"=>["config/environments"],
          "config/initializers"=>["config/initializers"],
          "config/locales"=>["config/locales"],
          "config/routes"=>["config/routes.rb"],
          "db"=>["db"],
          "db/migrate"=>["db/migrate"],
          "db/seeds"=>["db/seeds.rb"],
          "vendor"=>["vendor"],
          "vendor/assets"=>["vendor/assets"],
          "vendor/plugins"=>["vendor/plugins"]},
        @root=
         #<Pathname:/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/coffee-rails-3.2.2>>,
      @plugins=[]>>,
   #<Jquery::Rails::Engine:0x007ff8c62aef60
    @_all_autoload_paths=[],
    @_all_load_paths=
     ["/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/jquery-rails-2.1.4/lib",
      "/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/jquery-rails-2.1.4/vendor"],
    @config=
     #<Rails::Engine::Configuration:0x007ff8c6155e98
      @autoload_once_paths=[],
      @autoload_paths=[],
      @eager_load_paths=[],
      @generators=
       #<Rails::Configuration::Generators:0x007ff8c6155e70
        @aliases={},
        @colorize_logging=true,
        @fallbacks={},
        @hidden_namespaces=["sass"],
        @options=
         {:rails=>
           {:orm=>:active_record,
            :test_framework=>:test_unit,
            :integration_tool=>:test_unit,
            :performance_tool=>:test_unit,
            :stylesheet_engine=>:scss,
            :javascript_engine=>:coffee},
          :active_record=>{:migration=>true, :timestamps=>true},
          :test_unit=>{:fixture=>true, :fixture_replacement=>nil}},
        @templates=[]>,
      @paths=
       {"app"=>["app"],
        "app/assets"=>["app/assets"],
        "app/controllers"=>["app/controllers"],
        "app/helpers"=>["app/helpers"],
        "app/models"=>["app/models"],
        "app/mailers"=>["app/mailers"],
        "app/views"=>["app/views"],
        "lib"=>["lib"],
        "lib/assets"=>["lib/assets"],
        "lib/tasks"=>["lib/tasks"],
        "config"=>["config"],
        "config/environments"=>["config/environments"],
        "config/initializers"=>["config/initializers"],
        "config/locales"=>["config/locales"],
        "config/routes"=>["config/routes.rb"],
        "db"=>["db"],
        "db/migrate"=>["db/migrate"],
        "db/seeds"=>["db/seeds.rb"],
        "vendor"=>["vendor"],
        "vendor/assets"=>["vendor/assets"],
        "vendor/plugins"=>["vendor/plugins"]},
      @root=
       #<Pathname:/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/jquery-rails-2.1.4>>,
    @initializers=
     [#<Rails::Initializable::Initializer:0x007ff8c61d34d8
       @block=
        #<Proc:0x007ff8c3a0a2a8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:524>,
       @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
       @name=:set_load_path,
       @options={:before=>:bootstrap_hook, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c61d3488
       @block=
        #<Proc:0x007ff8c3a0a118@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:536>,
       @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
       @name=:set_autoload_paths,
       @options=
        {:before=>:bootstrap_hook, :after=>:set_load_path, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c61d3410
       @block=
        #<Proc:0x007ff8c3a09f38@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:546>,
       @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
       @name=:add_routing_paths,
       @options={:after=>:set_autoload_paths, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c61d3398
       @block=
        #<Proc:0x007ff8c3a09da8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:557>,
       @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
       @name=:add_locales,
       @options={:after=>:add_routing_paths, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c61d3348
       @block=
        #<Proc:0x007ff8c3a09bc8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:561>,
       @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
       @name=:add_view_paths,
       @options={:after=>:add_locales, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c61d32d0
       @block=
        #<Proc:0x007ff8c3a099e8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:569>,
       @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
       @name=:load_environment_config,
       @options=
        {:before=>:load_environment_hook,
         :group=>:all,
         :after=>:add_view_paths}>,
      #<Rails::Initializable::Initializer:0x007ff8c61d3258
       @block=
        #<Proc:0x007ff8c3a09858@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:574>,
       @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
       @name=:append_assets_path,
       @options={:group=>:all, :after=>:load_environment_config}>,
      #<Rails::Initializable::Initializer:0x007ff8c61d3208
       @block=
        #<Proc:0x007ff8c3a09678@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:580>,
       @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
       @name=:prepend_helpers_path,
       @options={:after=>:append_assets_path, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c61d3190
       @block=
        #<Proc:0x007ff8c3a093f8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:586>,
       @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
       @name=:load_config_initializers,
       @options={:after=>:prepend_helpers_path, :group=>:default}>,
      #<Rails::Initializable::Initializer:0x007ff8c61d3118
       @block=
        #<Proc:0x007ff8c3a09218@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:592>,
       @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
       @name=:engines_blank_point,
       @options={:after=>:load_config_initializers, :group=>:default}>],
    @railties=
     #<Rails::Engine::Railties:0x007ff8c6155a10
      @all=[],
      @config=
       #<Rails::Engine::Configuration:0x007ff8c6155e98
        @autoload_once_paths=[],
        @autoload_paths=[],
        @eager_load_paths=[],
        @generators=
         #<Rails::Configuration::Generators:0x007ff8c6155e70
          @aliases={},
          @colorize_logging=true,
          @fallbacks={},
          @hidden_namespaces=["sass"],
          @options=
           {:rails=>
             {:orm=>:active_record,
              :test_framework=>:test_unit,
              :integration_tool=>:test_unit,
              :performance_tool=>:test_unit,
              :stylesheet_engine=>:scss,
              :javascript_engine=>:coffee},
            :active_record=>{:migration=>true, :timestamps=>true},
            :test_unit=>{:fixture=>true, :fixture_replacement=>nil}},
          @templates=[]>,
        @paths=
         {"app"=>["app"],
          "app/assets"=>["app/assets"],
          "app/controllers"=>["app/controllers"],
          "app/helpers"=>["app/helpers"],
          "app/models"=>["app/models"],
          "app/mailers"=>["app/mailers"],
          "app/views"=>["app/views"],
          "lib"=>["lib"],
          "lib/assets"=>["lib/assets"],
          "lib/tasks"=>["lib/tasks"],
          "config"=>["config"],
          "config/environments"=>["config/environments"],
          "config/initializers"=>["config/initializers"],
          "config/locales"=>["config/locales"],
          "config/routes"=>["config/routes.rb"],
          "db"=>["db"],
          "db/migrate"=>["db/migrate"],
          "db/seeds"=>["db/seeds.rb"],
          "vendor"=>["vendor"],
          "vendor/assets"=>["vendor/assets"],
          "vendor/plugins"=>["vendor/plugins"]},
        @root=
         #<Pathname:/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/jquery-rails-2.1.4>>,
      @plugins=[]>>,
   #<SampleApp::Application:0x007ff8c3a19708 ...>],
 @railties=
  #<Rails::Application::Railties:0x007ff8c62af0f0
   @all=
    [#<I18n::Railtie:0x007ff8c6070500
      @config=#<Rails::Railtie::Configuration:0x007ff8c60c1720>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c614c550
         @block=
          #<Proc:0x007ff8c60c0f50@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/i18n_railtie.rb:24>,
         @context=#<I18n::Railtie:0x007ff8c6070500 ...>,
         @name="i18n.callbacks",
         @options={:group=>:default}>]>,
     #<ActiveSupport::Railtie:0x007ff8c60c0a50
      @config=#<Rails::Railtie::Configuration:0x007ff8c60c0a28>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c614c230
         @block=
          #<Proc:0x007ff8c60c0848@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/railtie.rb:10>,
         @context=#<ActiveSupport::Railtie:0x007ff8c60c0a50 ...>,
         @name="active_support.initialize_whiny_nils",
         @options={:group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c614c1e0
         @block=
          #<Proc:0x007ff8c60c0758@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/railtie.rb:14>,
         @context=#<ActiveSupport::Railtie:0x007ff8c60c0a50 ...>,
         @name="active_support.deprecation_behavior",
         @options=
          {:after=>"active_support.initialize_whiny_nils", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c614c168
         @block=
          #<Proc:0x007ff8c60c0668@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/railtie.rb:46>,
         @context=#<ActiveSupport::Railtie:0x007ff8c60c0a50 ...>,
         @name="active_support.initialize_time_zone",
         @options=
          {:after=>"active_support.deprecation_behavior", :group=>:default}>]>,
     #<ActionDispatch::Railtie:0x007ff8c610c770
      @config=#<Rails::Railtie::Configuration:0x007ff8c610c748>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c614be48
         @block=
          #<Proc:0x007ff8c61281c8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_dispatch/railtie.rb:22>,
         @context=#<ActionDispatch::Railtie:0x007ff8c610c770 ...>,
         @name="action_dispatch.configure",
         @options={:group=>:default}>]>,
     #<ActionView::Railtie:0x007ff8c3760b10
      @config=#<Rails::Railtie::Configuration:0x007ff8c3760ae8>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c614bab0
         @block=
          #<Proc:0x007ff8c37602c8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_view/railtie.rb:12>,
         @context=#<ActionView::Railtie:0x007ff8c3760b10 ...>,
         @name="action_view.embed_authenticity_token_in_remote_forms",
         @options={:group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c614ba38
         @block=
          #<Proc:0x007ff8c3760160@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_view/railtie.rb:19>,
         @context=#<ActionView::Railtie:0x007ff8c3760b10 ...>,
         @name="action_view.cache_asset_ids",
         @options=
          {:after=>"action_view.embed_authenticity_token_in_remote_forms",
           :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c614b9e8
         @block=
          #<Proc:0x007ff8c375fff8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_view/railtie.rb:27>,
         @context=#<ActionView::Railtie:0x007ff8c3760b10 ...>,
         @name="action_view.javascript_expansions",
         @options={:after=>"action_view.cache_asset_ids", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c614b970
         @block=
          #<Proc:0x007ff8c375feb8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_view/railtie.rb:39>,
         @context=#<ActionView::Railtie:0x007ff8c3760b10 ...>,
         @name="action_view.set_configs",
         @options=
          {:after=>"action_view.javascript_expansions", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c614b920
         @block=
          #<Proc:0x007ff8c375fdc8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_view/railtie.rb:47>,
         @context=#<ActionView::Railtie:0x007ff8c3760b10 ...>,
         @name="action_view.caching",
         @options={:after=>"action_view.set_configs", :group=>:default}>]>,
     #<ActionController::Railtie:0x007ff8c3697328
      @config=#<Rails::Railtie::Configuration:0x007ff8c3697300>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c614b560
         @block=
          #<Proc:0x007ff8c3697030@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/railtie.rb:12>,
         @context=#<ActionController::Railtie:0x007ff8c3697328 ...>,
         @name="action_controller.logger",
         @options={:group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c614b4e8
         @block=
          #<Proc:0x007ff8c3696ef0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/railtie.rb:16>,
         @context=#<ActionController::Railtie:0x007ff8c3697328 ...>,
         @name="action_controller.initialize_framework_caches",
         @options={:after=>"action_controller.logger", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c614b498
         @block=
          #<Proc:0x007ff8c3696d88@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/railtie.rb:20>,
         @context=#<ActionController::Railtie:0x007ff8c3697328 ...>,
         @name="action_controller.assets_config",
         @options=
          {:group=>:all,
           :after=>"action_controller.initialize_framework_caches"}>,
        #<Rails::Initializable::Initializer:0x007ff8c614b420
         @block=
          #<Proc:0x007ff8c3696cc0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/railtie.rb:24>,
         @context=#<ActionController::Railtie:0x007ff8c3697328 ...>,
         @name="action_controller.set_configs",
         @options=
          {:after=>"action_controller.assets_config", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c61533a0
         @block=
          #<Proc:0x007ff8c3696ba8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_controller/railtie.rb:45>,
         @context=#<ActionController::Railtie:0x007ff8c3697328 ...>,
         @name="action_controller.compile_config_methods",
         @options=
          {:after=>"action_controller.set_configs", :group=>:default}>]>,
     #<ActiveRecord::Railtie:0x007ff8c3696838
      @config=#<Rails::Railtie::Configuration:0x007ff8c3696810>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c6152fb8
         @block=
          #<Proc:0x007ff8c3695e88@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:44>,
         @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
         @name="active_record.initialize_timezone",
         @options={:group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6152f68
         @block=
          #<Proc:0x007ff8c3695d48@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:51>,
         @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
         @name="active_record.logger",
         @options=
          {:after=>"active_record.initialize_timezone", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6152ef0
         @block=
          #<Proc:0x007ff8c3695c58@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:55>,
         @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
         @name="active_record.identity_map",
         @options={:after=>"active_record.logger", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6152ea0
         @block=
          #<Proc:0x007ff8c3695b40@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:60>,
         @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
         @name="active_record.set_configs",
         @options={:after=>"active_record.identity_map", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6152e28
         @block=
          #<Proc:0x007ff8c3695a28@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:73>,
         @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
         @name="active_record.initialize_database",
         @options={:after=>"active_record.set_configs", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6152dd8
         @block=
          #<Proc:0x007ff8c3695938@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:87>,
         @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
         @name="active_record.log_runtime",
         @options=
          {:after=>"active_record.initialize_database", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6152d60
         @block=
          #<Proc:0x007ff8c3695820@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:94>,
         @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
         @name="active_record.set_reloader_hooks",
         @options={:after=>"active_record.log_runtime", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6152ce8
         @block=
          #<Proc:0x007ff8c3695708@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/railtie.rb:111>,
         @context=#<ActiveRecord::Railtie:0x007ff8c3696838 ...>,
         @name="active_record.add_watchable_files",
         @options=
          {:after=>"active_record.set_reloader_hooks", :group=>:default}>]>,
     #<ActionMailer::Railtie:0x007ff8c3045cb8
      @config=#<Rails::Railtie::Configuration:0x007ff8c3045c90>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c61529a0
         @block=
          #<Proc:0x007ff8c30445c0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionmailer-3.2.11/lib/action_mailer/railtie.rb:9>,
         @context=#<ActionMailer::Railtie:0x007ff8c3045cb8 ...>,
         @name="action_mailer.logger",
         @options={:group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6152928
         @block=
          #<Proc:0x007ff8c3043760@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionmailer-3.2.11/lib/action_mailer/railtie.rb:13>,
         @context=#<ActionMailer::Railtie:0x007ff8c3045cb8 ...>,
         @name="action_mailer.set_configs",
         @options={:after=>"action_mailer.logger", :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c61528d8
         @block=
          #<Proc:0x007ff8c3046f50@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionmailer-3.2.11/lib/action_mailer/railtie.rb:38>,
         @context=#<ActionMailer::Railtie:0x007ff8c3045cb8 ...>,
         @name="action_mailer.compile_config_methods",
         @options={:after=>"action_mailer.set_configs", :group=>:default}>]>,
     #<ActiveResource::Railtie:0x007ff8c30c85a0
      @config=#<Rails::Railtie::Configuration:0x007ff8c30c8410>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c61525b8
         @block=
          #<Proc:0x007ff8c30ce5e0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activeresource-3.2.11/lib/active_resource/railtie.rb:8>,
         @context=#<ActiveResource::Railtie:0x007ff8c30c85a0 ...>,
         @name="active_resource.set_configs",
         @options={:group=>:default}>]>,
     #<Rails::TestUnitRailtie:0x007ff8c30e7d88
      @config=#<Rails::Railtie::Configuration:0x007ff8c30e7d60>,
      @initializers=[]>,
     #<Sprockets::Railtie:0x007ff8c317b7e0
      @config=#<Rails::Railtie::Configuration:0x007ff8c317b420>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c6151f78
         @block=
          #<Proc:0x007ff8c317bab0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/sprockets/railtie.rb:17>,
         @context=#<Sprockets::Railtie:0x007ff8c317b7e0 ...>,
         @name="sprockets.environment",
         @options={:group=>:all}>]>,
     #<Sass::Rails::Railtie:0x007ff8c37ac8d0
      @config=#<Rails::Railtie::Configuration:0x007ff8c37ac880>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c6151c58
         @block=
          #<Proc:0x007ff8c610c5b8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/sass-rails-3.2.6/lib/sass/rails/railtie.rb:47>,
         @context=#<Sass::Rails::Railtie:0x007ff8c37ac8d0 ...>,
         @name=:setup_sass,
         @options={:group=>:all}>,
        #<Rails::Initializable::Initializer:0x007ff8c6151be0
         @block=
          #<Proc:0x007ff8c610c4f0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/sass-rails-3.2.6/lib/sass/rails/railtie.rb:73>,
         @context=#<Sass::Rails::Railtie:0x007ff8c37ac8d0 ...>,
         @name=:setup_compression,
         @options={:group=>:all, :after=>:setup_sass}>]>,
     #<Jquery::Rails::Railtie:0x007ff8c31de3e0
      @config=#<Rails::Railtie::Configuration:0x007ff8c31de0e8>,
      @initializers=[]>,
     #<Coffee::Rails::Engine:0x007ff8c3d9b9a8
      @_all_autoload_paths=[],
      @_all_load_paths=
       ["/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/coffee-rails-3.2.2/lib"],
      @config=
       #<Rails::Engine::Configuration:0x007ff8c480eca0
        @autoload_once_paths=[],
        @autoload_paths=[],
        @eager_load_paths=[],
        @generators=
         #<Rails::Configuration::Generators:0x007ff8c480ec28
          @aliases={},
          @colorize_logging=true,
          @fallbacks={},
          @hidden_namespaces=["sass"],
          @options=
           {:rails=>
             {:orm=>:active_record,
              :test_framework=>:test_unit,
              :integration_tool=>:test_unit,
              :performance_tool=>:test_unit,
              :stylesheet_engine=>:scss},
            :active_record=>{:migration=>true, :timestamps=>true},
            :test_unit=>{:fixture=>true, :fixture_replacement=>nil}},
          @templates=[]>,
        @paths=
         {"app"=>["app"],
          "app/assets"=>["app/assets"],
          "app/controllers"=>["app/controllers"],
          "app/helpers"=>["app/helpers"],
          "app/models"=>["app/models"],
          "app/mailers"=>["app/mailers"],
          "app/views"=>["app/views"],
          "lib"=>["lib"],
          "lib/assets"=>["lib/assets"],
          "lib/tasks"=>["lib/tasks"],
          "config"=>["config"],
          "config/environments"=>["config/environments"],
          "config/initializers"=>["config/initializers"],
          "config/locales"=>["config/locales"],
          "config/routes"=>["config/routes.rb"],
          "db"=>["db"],
          "db/migrate"=>["db/migrate"],
          "db/seeds"=>["db/seeds.rb"],
          "vendor"=>["vendor"],
          "vendor/assets"=>["vendor/assets"],
          "vendor/plugins"=>["vendor/plugins"]},
        @root=
         #<Pathname:/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/coffee-rails-3.2.2>>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c61570b8
         @block=
          #<Proc:0x007ff8c3a0a2a8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:524>,
         @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
         @name=:set_load_path,
         @options={:before=>:bootstrap_hook, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6157040
         @block=
          #<Proc:0x007ff8c3a0a118@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:536>,
         @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
         @name=:set_autoload_paths,
         @options=
          {:before=>:bootstrap_hook,
           :after=>:set_load_path,
           :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6156fc8
         @block=
          #<Proc:0x007ff8c3a09f38@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:546>,
         @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
         @name=:add_routing_paths,
         @options={:after=>:set_autoload_paths, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6156f78
         @block=
          #<Proc:0x007ff8c3a09da8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:557>,
         @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
         @name=:add_locales,
         @options={:after=>:add_routing_paths, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6156f00
         @block=
          #<Proc:0x007ff8c3a09bc8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:561>,
         @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
         @name=:add_view_paths,
         @options={:after=>:add_locales, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6156e88
         @block=
          #<Proc:0x007ff8c3a099e8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:569>,
         @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
         @name=:load_environment_config,
         @options=
          {:before=>:load_environment_hook,
           :group=>:all,
           :after=>:add_view_paths}>,
        #<Rails::Initializable::Initializer:0x007ff8c6156e38
         @block=
          #<Proc:0x007ff8c3a09858@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:574>,
         @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
         @name=:append_assets_path,
         @options={:group=>:all, :after=>:load_environment_config}>,
        #<Rails::Initializable::Initializer:0x007ff8c6156dc0
         @block=
          #<Proc:0x007ff8c3a09678@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:580>,
         @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
         @name=:prepend_helpers_path,
         @options={:after=>:append_assets_path, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6156d70
         @block=
          #<Proc:0x007ff8c3a093f8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:586>,
         @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
         @name=:load_config_initializers,
         @options={:after=>:prepend_helpers_path, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c6156cf8
         @block=
          #<Proc:0x007ff8c3a09218@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:592>,
         @context=#<Coffee::Rails::Engine:0x007ff8c3d9b9a8 ...>,
         @name=:engines_blank_point,
         @options={:after=>:load_config_initializers, :group=>:default}>],
      @railties=
       #<Rails::Engine::Railties:0x007ff8c61517f8
        @all=[],
        @config=
         #<Rails::Engine::Configuration:0x007ff8c480eca0
          @autoload_once_paths=[],
          @autoload_paths=[],
          @eager_load_paths=[],
          @generators=
           #<Rails::Configuration::Generators:0x007ff8c480ec28
            @aliases={},
            @colorize_logging=true,
            @fallbacks={},
            @hidden_namespaces=["sass"],
            @options=
             {:rails=>
               {:orm=>:active_record,
                :test_framework=>:test_unit,
                :integration_tool=>:test_unit,
                :performance_tool=>:test_unit,
                :stylesheet_engine=>:scss},
              :active_record=>{:migration=>true, :timestamps=>true},
              :test_unit=>{:fixture=>true, :fixture_replacement=>nil}},
            @templates=[]>,
          @paths=
           {"app"=>["app"],
            "app/assets"=>["app/assets"],
            "app/controllers"=>["app/controllers"],
            "app/helpers"=>["app/helpers"],
            "app/models"=>["app/models"],
            "app/mailers"=>["app/mailers"],
            "app/views"=>["app/views"],
            "lib"=>["lib"],
            "lib/assets"=>["lib/assets"],
            "lib/tasks"=>["lib/tasks"],
            "config"=>["config"],
            "config/environments"=>["config/environments"],
            "config/initializers"=>["config/initializers"],
            "config/locales"=>["config/locales"],
            "config/routes"=>["config/routes.rb"],
            "db"=>["db"],
            "db/migrate"=>["db/migrate"],
            "db/seeds"=>["db/seeds.rb"],
            "vendor"=>["vendor"],
            "vendor/assets"=>["vendor/assets"],
            "vendor/plugins"=>["vendor/plugins"]},
          @root=
           #<Pathname:/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/coffee-rails-3.2.2>>,
        @plugins=[]>>,
     #<Jquery::Rails::Engine:0x007ff8c62aef60
      @_all_autoload_paths=[],
      @_all_load_paths=
       ["/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/jquery-rails-2.1.4/lib",
        "/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/jquery-rails-2.1.4/vendor"],
      @config=
       #<Rails::Engine::Configuration:0x007ff8c6155e98
        @autoload_once_paths=[],
        @autoload_paths=[],
        @eager_load_paths=[],
        @generators=
         #<Rails::Configuration::Generators:0x007ff8c6155e70
          @aliases={},
          @colorize_logging=true,
          @fallbacks={},
          @hidden_namespaces=["sass"],
          @options=
           {:rails=>
             {:orm=>:active_record,
              :test_framework=>:test_unit,
              :integration_tool=>:test_unit,
              :performance_tool=>:test_unit,
              :stylesheet_engine=>:scss,
              :javascript_engine=>:coffee},
            :active_record=>{:migration=>true, :timestamps=>true},
            :test_unit=>{:fixture=>true, :fixture_replacement=>nil}},
          @templates=[]>,
        @paths=
         {"app"=>["app"],
          "app/assets"=>["app/assets"],
          "app/controllers"=>["app/controllers"],
          "app/helpers"=>["app/helpers"],
          "app/models"=>["app/models"],
          "app/mailers"=>["app/mailers"],
          "app/views"=>["app/views"],
          "lib"=>["lib"],
          "lib/assets"=>["lib/assets"],
          "lib/tasks"=>["lib/tasks"],
          "config"=>["config"],
          "config/environments"=>["config/environments"],
          "config/initializers"=>["config/initializers"],
          "config/locales"=>["config/locales"],
          "config/routes"=>["config/routes.rb"],
          "db"=>["db"],
          "db/migrate"=>["db/migrate"],
          "db/seeds"=>["db/seeds.rb"],
          "vendor"=>["vendor"],
          "vendor/assets"=>["vendor/assets"],
          "vendor/plugins"=>["vendor/plugins"]},
        @root=
         #<Pathname:/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/jquery-rails-2.1.4>>,
      @initializers=
       [#<Rails::Initializable::Initializer:0x007ff8c61d34d8
         @block=
          #<Proc:0x007ff8c3a0a2a8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:524>,
         @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
         @name=:set_load_path,
         @options={:before=>:bootstrap_hook, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c61d3488
         @block=
          #<Proc:0x007ff8c3a0a118@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:536>,
         @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
         @name=:set_autoload_paths,
         @options=
          {:before=>:bootstrap_hook,
           :after=>:set_load_path,
           :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c61d3410
         @block=
          #<Proc:0x007ff8c3a09f38@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:546>,
         @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
         @name=:add_routing_paths,
         @options={:after=>:set_autoload_paths, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c61d3398
         @block=
          #<Proc:0x007ff8c3a09da8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:557>,
         @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
         @name=:add_locales,
         @options={:after=>:add_routing_paths, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c61d3348
         @block=
          #<Proc:0x007ff8c3a09bc8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:561>,
         @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
         @name=:add_view_paths,
         @options={:after=>:add_locales, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c61d32d0
         @block=
          #<Proc:0x007ff8c3a099e8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:569>,
         @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
         @name=:load_environment_config,
         @options=
          {:before=>:load_environment_hook,
           :group=>:all,
           :after=>:add_view_paths}>,
        #<Rails::Initializable::Initializer:0x007ff8c61d3258
         @block=
          #<Proc:0x007ff8c3a09858@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:574>,
         @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
         @name=:append_assets_path,
         @options={:group=>:all, :after=>:load_environment_config}>,
        #<Rails::Initializable::Initializer:0x007ff8c61d3208
         @block=
          #<Proc:0x007ff8c3a09678@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:580>,
         @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
         @name=:prepend_helpers_path,
         @options={:after=>:append_assets_path, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c61d3190
         @block=
          #<Proc:0x007ff8c3a093f8@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:586>,
         @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
         @name=:load_config_initializers,
         @options={:after=>:prepend_helpers_path, :group=>:default}>,
        #<Rails::Initializable::Initializer:0x007ff8c61d3118
         @block=
          #<Proc:0x007ff8c3a09218@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/engine.rb:592>,
         @context=#<Jquery::Rails::Engine:0x007ff8c62aef60 ...>,
         @name=:engines_blank_point,
         @options={:after=>:load_config_initializers, :group=>:default}>],
      @railties=
       #<Rails::Engine::Railties:0x007ff8c6155a10
        @all=[],
        @config=
         #<Rails::Engine::Configuration:0x007ff8c6155e98
          @autoload_once_paths=[],
          @autoload_paths=[],
          @eager_load_paths=[],
          @generators=
           #<Rails::Configuration::Generators:0x007ff8c6155e70
            @aliases={},
            @colorize_logging=true,
            @fallbacks={},
            @hidden_namespaces=["sass"],
            @options=
             {:rails=>
               {:orm=>:active_record,
                :test_framework=>:test_unit,
                :integration_tool=>:test_unit,
                :performance_tool=>:test_unit,
                :stylesheet_engine=>:scss,
                :javascript_engine=>:coffee},
              :active_record=>{:migration=>true, :timestamps=>true},
              :test_unit=>{:fixture=>true, :fixture_replacement=>nil}},
            @templates=[]>,
          @paths=
           {"app"=>["app"],
            "app/assets"=>["app/assets"],
            "app/controllers"=>["app/controllers"],
            "app/helpers"=>["app/helpers"],
            "app/models"=>["app/models"],
            "app/mailers"=>["app/mailers"],
            "app/views"=>["app/views"],
            "lib"=>["lib"],
            "lib/assets"=>["lib/assets"],
            "lib/tasks"=>["lib/tasks"],
            "config"=>["config"],
            "config/environments"=>["config/environments"],
            "config/initializers"=>["config/initializers"],
            "config/locales"=>["config/locales"],
            "config/routes"=>["config/routes.rb"],
            "db"=>["db"],
            "db/migrate"=>["db/migrate"],
            "db/seeds"=>["db/seeds.rb"],
            "vendor"=>["vendor"],
            "vendor/assets"=>["vendor/assets"],
            "vendor/plugins"=>["vendor/plugins"]},
          @root=
           #<Pathname:/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/jquery-rails-2.1.4>>,
        @plugins=[]>>],
   @config=
    #<Rails::Application::Configuration:0x007ff8c3b11110
     @allow_concurrency=false,
     @assets=
      {:enabled=>true,
       :paths=>
        ["/Users/Altech/dev/reading/sample_app/app/assets/images",
         "/Users/Altech/dev/reading/sample_app/app/assets/javascripts",
         "/Users/Altech/dev/reading/sample_app/app/assets/stylesheets",
         "/Users/Altech/dev/reading/sample_app/vendor/assets/javascripts",
         "/Users/Altech/dev/reading/sample_app/vendor/assets/stylesheets",
         "/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/jquery-rails-2.1.4/vendor/assets/javascripts",
         "/Users/Altech/.rvm/gems/ruby-1.9.3-p286/gems/coffee-rails-3.2.2/lib/assets/javascripts"],
       :precompile=>
        [#<Proc:0x007ff8c3b0eaa0@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/application/configuration.rb:48>,
         /(?:\/|\\|\A)application\.(css|js)$/],
       :prefix=>"/assets",
       :version=>"1.0",
       :debug=>true,
       :compile=>true,
       :digest=>false,
       :manifest=>nil,
       :cache_store=>
        [:file_store,
         "/Users/Altech/dev/reading/sample_app/tmp/cache/assets/"],
       :js_compressor=>nil,
       :css_compressor=>nil,
       :initialize_on_precompile=>true,
       :logger=>nil,
       :compress=>false},
     @autoload_once_paths=[],
     @autoload_paths=[],
     @cache_classes=false,
     @cache_store=
      [:file_store, "/Users/Altech/dev/reading/sample_app/tmp/cache/"],
     @consider_all_requests_local=true,
     @dependency_loading=true,
     @eager_load_paths=
      ["/Users/Altech/dev/reading/sample_app/app/assets",
       "/Users/Altech/dev/reading/sample_app/app/controller",
       "/Users/Altech/dev/reading/sample_app/app/controllers",
       "/Users/Altech/dev/reading/sample_app/app/helpers",
       "/Users/Altech/dev/reading/sample_app/app/mailers",
       "/Users/Altech/dev/reading/sample_app/app/models"],
     @encoding="utf-8",
     @exceptions_app=nil,
     @file_watcher=ActiveSupport::FileUpdateChecker,
     @filter_parameters=[:password],
     @force_ssl=false,
     @generators=
      #<Rails::Configuration::Generators:0x007ff8c3696658
       @aliases={},
       @colorize_logging=true,
       @fallbacks={},
       @hidden_namespaces=["sass"],
       @options=
        {:rails=>
          {:orm=>:active_record,
           :test_framework=>:test_unit,
           :integration_tool=>:test_unit,
           :performance_tool=>:test_unit,
           :stylesheet_engine=>:scss,
           :javascript_engine=>:coffee},
         :active_record=>{:migration=>true, :timestamps=>true},
         :test_unit=>{:fixture=>true, :fixture_replacement=>nil}},
       @templates=[]>,
     @helpers_paths=["/Users/Altech/dev/reading/sample_app/app/helpers"],
     @log_level=:debug,
     @middleware=
      #<ActionDispatch::MiddlewareStack:0x007ff8c377c8d8
       @middlewares=
        [ActionDispatch::Static,
         Rack::Lock,
         #<ActiveSupport::Cache::Strategy::LocalCache::Middleware:0x007ff8c36951b8>,
         Rack::Runtime,
         Rack::MethodOverride,
         ActionDispatch::RequestId,
         Rails::Rack::Logger,
         ActionDispatch::ShowExceptions,
         ActionDispatch::DebugExceptions,
         ActionDispatch::RemoteIp,
         ActionDispatch::Reloader,
         ActionDispatch::Callbacks,
         ActiveRecord::ConnectionAdapters::ConnectionManagement,
         ActiveRecord::QueryCache,
         ActionDispatch::Cookies,
         ActionDispatch::Session::CookieStore,
         ActionDispatch::Flash,
         ActionDispatch::ParamsParser,
         ActionDispatch::Head,
         Rack::ConditionalGet,
         Rack::ETag,
         ActionDispatch::BestStandardsSupport]>,
     @paths=
      {"app"=>["app"],
       "app/assets"=>["app/assets"],
       "app/controllers"=>["app/controllers"],
       "app/helpers"=>["app/helpers"],
       "app/models"=>["app/models"],
       "app/mailers"=>["app/mailers"],
       "app/views"=>["app/views"],
       "lib"=>["lib"],
       "lib/assets"=>["lib/assets"],
       "lib/tasks"=>["lib/tasks"],
       "config"=>["config"],
       "config/environments"=>["config/environments"],
       "config/initializers"=>["config/initializers"],
       "config/locales"=>["config/locales"],
       "config/routes"=>["config/routes.rb"],
       "db"=>["db"],
       "db/migrate"=>["db/migrate"],
       "db/seeds"=>["db/seeds.rb"],
       "vendor"=>["vendor"],
       "vendor/assets"=>["vendor/assets"],
       "vendor/plugins"=>["vendor/plugins"],
       "config/database"=>["config/database.yml"],
       "config/environment"=>["config/environment.rb"],
       "lib/templates"=>["lib/templates"],
       "log"=>["log/development.log"],
       "public"=>["public"],
       "public/javascripts"=>["public/javascripts"],
       "public/stylesheets"=>["public/stylesheets"],
       "tmp"=>["tmp"]},
     @railties_order=[:all],
     @relative_url_root=nil,
     @reload_classes_only_on_change=true,
     @root=#<Pathname:/Users/Altech/dev/reading/sample_app>,
     @secret_token=
      "71b16ed4a690561f778ebb488e51588a561d7bbcff10f98b1e7d641cff8724fa79f9047581c67890e67550a2bd180fd8bb295f9351430ac2577f874f7fc1891b",
     @serve_static_assets=true,
     @session_options=
      {:key=>"_sample_app_session",
       :secret=>"7dc802f779c58d5b6f87c123f0ab78b12fdda4a56bb33c8f03d4bfdee551",
       :coder=>#<Rack::Session::Cookie::Base64::Marshal:0x007ff8c634c4e0>,
       :cookie_only=>true},
     @session_store=:cookie_store,
     @ssl_options={},
     @static_cache_control=nil,
     @time_zone="UTC",
     @whiny_nils=true>,
   @plugins=[]>,
 @ran=true,
 @reloaders=
  [#<ActiveSupport::FileUpdateChecker:0x007ff8c370f850
    @block=
     #<Proc:0x007ff8c370f760@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/i18n_railtie.rb:13>,
    @files=
     ["/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activesupport-3.2.11/lib/active_support/locale/en.yml",
      "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activemodel-3.2.11/lib/active_model/locale/en.yml",
      "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/activerecord-3.2.11/lib/active_record/locale/en.yml",
      "/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/actionpack-3.2.11/lib/action_view/locale/en.yml",
      "/Users/Altech/dev/reading/sample_app/config/locales/en.yml"],
    @glob=nil,
    @last_update_at=2013-01-18 19:18:04 +0900,
    @updated_at=nil>,
   #<Rails::Application::RoutesReloader:0x007ff8c612a0b8
    @paths=["/Users/Altech/dev/reading/sample_app/config/routes.rb"],
    @route_sets=[#<ActionDispatch::Routing::RouteSet:0x007ff8c62aa320>],
    @updater=
     #<ActiveSupport::FileUpdateChecker:0x007ff8c3b983e0
      @block=
       #<Proc:0x007ff8c3b98390@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/application/routes_reloader.rb:26>,
      @files=["/Users/Altech/dev/reading/sample_app/config/routes.rb"],
      @glob=nil,
      @last_update_at=2013-01-31 20:17:01 +0900,
      @updated_at=nil>>,
   #<ActiveSupport::FileUpdateChecker:0x007ff8c6336aa0
    @block=
     #<Proc:0x007ff8c6336d98@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/application/finisher.rb:74 (lambda)>,
    @files=
     ["/Users/Altech/dev/reading/sample_app/db/schema.rb",
      "/Users/Altech/dev/reading/sample_app/db/structure.sql"],
    @glob=
     "{/Users/Altech/dev/reading/sample_app/app/assets/**/*.{rb},/Users/Altech/dev/reading/sample_app/app/controller/**/*.{rb},/Users/Altech/dev/reading/sample_app/app/controllers/**/*.{rb},/Users/Altech/dev/reading/sample_app/app/helpers/**/*.{rb},/Users/Altech/dev/reading/sample_app/app/mailers/**/*.{rb},/Users/Altech/dev/reading/sample_app/app/models/**/*.{rb}}",
    @last_update_at=2013-02-19 20:36:40 +0900,
    @updated_at=nil>],
 @routes=#<ActionDispatch::Routing::RouteSet:0x007ff8c62aa320>,
 @routes_reloader=
  #<Rails::Application::RoutesReloader:0x007ff8c612a0b8
   @paths=["/Users/Altech/dev/reading/sample_app/config/routes.rb"],
   @route_sets=[#<ActionDispatch::Routing::RouteSet:0x007ff8c62aa320>],
   @updater=
    #<ActiveSupport::FileUpdateChecker:0x007ff8c3b983e0
     @block=
      #<Proc:0x007ff8c3b98390@/Users/Altech/.rvm/rubies/ruby-1.9.3-p286/lib/ruby/gems/1.9.1/gems/railties-3.2.11/lib/rails/application/routes_reloader.rb:26>,
     @files=["/Users/Altech/dev/reading/sample_app/config/routes.rb"],
     @glob=nil,
     @last_update_at=2013-01-31 20:17:01 +0900,
     @updated_at=nil>>>
