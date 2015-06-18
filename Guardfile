# A sample Guardfile
# More info at https://github.com/guard/guard#readme


# guard 'compass', project_path: 'not_current_dir', configuration_file: 'path/to/my/compass_config.rb'
guard :compass

guard 'ctags-bundler', :src_path => ["app", "lib", "spec/support"] do
  watch(/^(app|lib|spec\/support)\/.*\.rb$/)
  watch('Gemfile.lock')
end

guard 'livereload' do
  watch(%r{web/.+\.(css|js|html)})
end
