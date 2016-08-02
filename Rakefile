require "parallel_tests/tasks"

task :parallel do
  Rake::Task["parallel:features"].invoke(
    2,
    nil,
    "--require features features/nested_features"
  )
end
