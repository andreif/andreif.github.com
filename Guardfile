# A sample Guardfile
# More info at https://github.com/guard/guard#readme

# guard 'coffeescript', :input => 'app/assets/javascripts'#, :output => 'javascripts'
guard 'coffeescript', :output => 'public/javascripts/compiled' do
  watch(%r{app/coffeescripts/(.+\.coffee)})
  watch(%r{lib/coffeescripts/(.+\.coffee)})
end

guard 'compass' do
  watch('^src/(.*)\.s[ac]ss')
end

guard 'haml', :output => 'public', :input => 'src' do
  # watch(/^.+(\.html\.haml)/)
  watch %r{^src/.+(\.html\.haml)}
end

# https://github.com/guard/guard-jammit

guard 'bundler' do
  watch('Gemfile')
  # Uncomment next line if Gemfile contain `gemspec' command
  # watch(/^.+\.gemspec/)
end
