source 'https://rubygems.org'

gem 'rake'

group :test do
  gem 'backports'
  gem 'coveralls'
  gem 'mime-types', '~> 1.25', platforms: %i[jruby ruby_18]
  gem 'rest-client', '~> 1.6.0', platforms: %i[jruby ruby_18]
  gem 'rspec', '>= 3'
  gem 'rubocop', '0.65.0'
  gem 'simplecov', '>= 0.9'
end

case version = ENV['MONGOID_VERSION'] || '7.0'
when /^7/
  gem 'mongoid', '~> 7.0'
when /^6/
  gem 'mongoid', '~> 6.0'
when /^5/
  gem 'mongoid', '~> 5.0'
else
  gem 'mongoid', version
end

gemspec
