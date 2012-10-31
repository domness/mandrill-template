# encoding: utf-8

require 'rubygems'
require 'bundler'
Bundler::GemHelper.install_tasks
require 'rspec/core/rake_task'

require 'jeweler'
Jeweler::Tasks.new do |gem|
  # gem is a Gem::Specification... see http://docs.rubygems.org/read/chapter/20 for more options
  gem.name = "mandrill-template"
  gem.homepage = "http://github.com/domness/mandrill-template"
  gem.license = "MIT"
  gem.summary = %Q{Simple interface to Mandrill template api}
  gem.description = %Q{Simple interface to Mandrill template api}
  gem.email = "domness@gmail.com"
  gem.authors = ["Dominic Wroblewski"]
  # dependencies defined in Gemfile
end
Jeweler::RubygemsDotOrgTasks.new

RSpec::Core::RakeTask.new(:spec)

task :test => :spec
task :default => :spec

require 'rdoc/task'
Rake::RDocTask.new do |rdoc|
  version = File.exist?('VERSION') ? File.read('VERSION') : ""

  rdoc.rdoc_dir = 'rdoc'
  rdoc.title = "mandrill-template #{version}"
  rdoc.rdoc_files.include('README*')
  rdoc.rdoc_files.include('lib/**/*.rb')
end
