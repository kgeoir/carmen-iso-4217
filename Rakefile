require 'bundler/gem_tasks'
require 'rspec/core/rake_task'

Dir.glob('tasks/*.rake').each { |r| import r }

RSpec::Core::RakeTask.new(:spec)

task default: :spec

task :console do
  exec 'pry -r iso_4217 -I ./lib/carmen'
end
