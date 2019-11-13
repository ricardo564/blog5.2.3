redis: redis-server config/redis/development.conf
sidekiq: bundle exec sidekiq -v
sidekiq_web: bundle exec thin -R sidekiq.ru start -p 9292
mailcatcher: bundle exec mailcatcher --http-ip 0.0.0.0 -f
jasmine: bundle exec rake jasmine
web: bundle exec rails s
web: bundle exec unicorn -p $PORT -c ./config/unicorn.rb
worker: bundle exec rake worker --trace