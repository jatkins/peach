require 'rubygems'
require 'rake'
require 'rake/testtask'

Rake::TestTask.new(:test) do |t|
  t.libs << 'lib'
  t.pattern = 'test/*_test.rb'
  t.verbose = true
end

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gemspec|
    gemspec.name = "peach"
    gemspec.summary = "Parallel Each and other parallel things"
    gemspec.description = "Parallel Each and other parallel things"
    gemspec.email = "ben@pixelmachine.org"
    gemspec.homepage = "http://peach.rubyforge.org"
    gemspec.authors = ["Ben Hughes"]
  end
  Jeweler::GemcutterTasks.new
rescue LoadError  
  puts "Jeweler not available. Install it with: sudo gem install technicalpickles-jeweler -s http://gems.github.com"  
end

Dir["#{File.dirname(__FILE__)}/tasks/*.rake"].sort.each { |ext| load ext }  
