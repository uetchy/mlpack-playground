new_git_repository(
	name = "mlpack",
    remote = "https://github.com/mlpack/mlpack.git",
    tag = "mlpack-2.1.1",
    build_file_content = """
cc_library(
    name = "core",
    srcs = ["src/mlpack/core.hpp"],
    hdrs = ["src/mlpack/core.hpp"],
    visibility = ["//visibility:public"]
)"""
)

new_local_repository(
    name = "hdf5",
    path = "/usr/local/opt/hdf5",
    build_file_content = """
cc_library(
    name = "hdf5",
    srcs = glob(['/usr/local/opt/hdf5/lib/**']),
    hdrs = ["/usr/local/opt/hdf5/include/hdf5.h"],
    visibility = ["//visibility:public"]
)"""
)