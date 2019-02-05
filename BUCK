load('//:buckaroo_macros.bzl', 'buckaroo_deps')
load('//:subdir_glob.bzl', 'subdir_glob')

cxx_library(
  name = 'test',
  header_namespace = 'boost',
  exported_headers = subdir_glob([
    ('include/boost', '**/*.hpp'),
    ('include/boost', '**/*.ipp'),
  ]),
  srcs = glob([
    'src/**/*.cpp',
  ]),
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)
