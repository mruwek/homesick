require 'rbconfig'
source 'https://rubygems.org'

# Add dependencies required to use your gem here.
gem "thor", ">= 0.14.0"

# Add dependencies to develop your gem here.
# Include everything needed to run rake, tests, features, etc.
group :development do
  gem "rake", ">= 0.8.7"
  gem "rspec", "~> 3.5.0"
  gem "guard"
  gem "guard-rspec"
  gem "rb-readline", "~> 0.5.0"
  gem "test_construct"
  gem "capture-output", "~> 1.0.0"
  if RbConfig::CONFIG['host_os'] =~ /linux|freebsd|openbsd|sunos|solaris/
    gem 'libnotify'
  end
  if RbConfig::CONFIG['host_os'] =~ /darwin|mac os/
    gem 'terminal-notifier-guard', '~> 1.6.1'
  end
  gem "coveralls", require: false
  gem "rubocop"
  if RUBY_VERSION < '2.3.0'
    gem "rack", "< 2"
    gem "listen", "< 3"
    gem "jeweler", ">= 1.6.2", "< 2.2"
  else
    gem "jeweler", ">= 1.6.2"
  end
end
