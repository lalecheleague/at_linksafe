require 'rake'
require 'rake/testtask'
require "bundler/gem_tasks"

# see http://rake.rubyforge.org/classes/Rake/TestTask.html
# Run tests with:
#   $ cd at_linksafe
#   $ rake test
#
desc 'Run the ruby-openid tests.'
Rake::TestTask.new(:test) do |t|
  t.libs += ["lib", "test"]
  t.test_files = FileList['test/test_*.rb']
  t.verbose = true
end

desc 'Default: run unit tests.'
task :default => :test
