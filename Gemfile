source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end
# Heroku should use this version of ruby
ruby '2.3.3'

gem 'rails', '~> 5.1.2'

# sqlite3 for development and test database
gem 'sqlite3', group: [:development, :test]

# postgres for production database
gem 'pg', group: :production
# stripe for taking payments
gem 'stripe', '~> 3.0', '>= 3.0.1'
#12 factor for heroku
gem 'rails_12factor', group: :production

# activeadmin for admin system
gem 'activeadmin', github: 'activeadmin'
gem 'inherited_resources', github: 'activeadmin/inherited_resources'

# devise for user authentication
gem 'devise'
gem 'bcrypt', '~> 3.1', '>= 3.1.11'

# add twitter bootstrap
gem 'bootstrap-sass', '~> 3.3', '>= 3.3.7'
gem 'figaro'
gem 'letter_opener', group: :development
gem 'puma', '~> 3.7'
gem 'sass-rails', '~> 5.0'
gem 'uglifier', '>= 1.3.0'
gem 'coffee-script-source', '1.8.0'
gem 'coffee-rails', '~> 4.2'
gem 'turbolinks', '~> 5'
gem 'jbuilder', '~> 2.5'



group :development, :test do
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
  gem 'capybara', '~> 2.13'
  gem 'selenium-webdriver'
end

group :development do
  gem 'web-console', '>= 3.3.0'
end

gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
