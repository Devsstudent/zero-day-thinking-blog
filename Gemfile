# AGGRESSIVE Ruby 4.0 compatibility monkeypatch
# Re-defining methods removed in Ruby 3.2+ that are still required by Liquid 4.x
[Object, String].each do |klass|
  klass.send(:define_method, :untaint) { self }
  klass.send(:define_method, :taint) { self }
  klass.send(:define_method, :tainted?) { false }
end

source "https://rubygems.org"

# Ruby 4.0 compatibility
gem "jekyll", "~> 4.3"
gem "minima", "~> 2.5"

# Essential plugins
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-seo-tag"
  gem "jekyll-sitemap"
  gem "jekyll-remote-theme"
end

# Missing gems in Ruby 3.4+ default library
gem "csv"
gem "bigdecimal"
gem "base64"
gem "mutex_m"
gem "webrick"
gem "logger"
gem "ostruct"

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]
