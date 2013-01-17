source "http://rubygems.org"

gemspec

if ENV["edge"]
  gem "activerecord", :github => "rails/rails"
  gem "active_record_deprecated_finders", :github => "rails/active_record_deprecated_finders"
end

group :development do
  gem "rake"
  gem "yard"

  platforms :ruby do
    gem "sqlite3"
    gem "redcarpet"
  end

  platforms :jruby do
    gem "activerecord-jdbcsqlite3-adapter"
    gem "jruby-openssl", :require => false # Silence openssl warnings.
  end
end
