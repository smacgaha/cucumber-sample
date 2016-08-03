require "parallel_tests/tasks"

task :parallel do
  directory = "features/nested_features"
  count = 2
  cucumber_opts = nil

  directory_arg = directory || "features"
  count_arg = count ? "-n #{count}" : nil
  cucumber_opts_arg = cucumber_opts ? "-o #{cucumber_opts}" : nil

  command = "parallel_cucumber #{directory} #{count_arg} #{cucumber_opts_arg}"
  system(command)
end
