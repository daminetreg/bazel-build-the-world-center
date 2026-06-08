load("@rules_cc//cc:defs.bzl", "cc_library")

filegroup(
    name = "all_headers",
    srcs = glob([
        "include/**/*.hpp",
        "include/**/*.h",
    ]),
    visibility = ["//visibility:public"],
)

cc_library(
    name = "boost_core",
    hdrs = [":all_headers"],
    includes = ["include"],
    strip_include_prefix = "include",
    visibility = ["//visibility:public"],
)
