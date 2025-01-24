require "rspec/core/rake_task"

task :default => :run

# Development task that includes testing
task :dev => [:test]

# Run the project
task :run do
  puts "Running the project..."
end

# RSpec task
RSpec::Core::RakeTask.new(:spec) do |t|
  t.pattern = "spec/**/*_spec.rb" # Run all test files in the spec directory
end

# Task to run tests using `bundle exec rspec`
task :test do
  puts "Running tests..."
  sh "bundle exec rspec"
end
