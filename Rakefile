#!/usr/bin/env rake
require "bundler/gem_tasks"
require 'rspec/core/rake_task'

require 'rake/testtask'

Rake::TestTask.new do |t|
  t.libs.push "lib"
  t.libs.push "test"
  t.pattern = "test/**/*_test.rb"
  t.verbose = true
end

RSpec::Core::RakeTask.new(:spec)

task :default => :test
