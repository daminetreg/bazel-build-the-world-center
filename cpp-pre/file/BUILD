load("@rules_cc//cc:defs.bzl", "cc_library", "cc_test")

cc_library(
    name = "pre_file",
    hdrs = [
        "pre/file/hash.hpp",
        "pre/file/home.hpp",
        "pre/file/string.hpp",
    ],
    includes = ["."],
    visibility = ["//visibility:public"],
)

cc_test(
    name = "hash_test",
    srcs = ["tests/hash.cpp"],
    hdrs = ["tests/util.hpp"],
    deps = [":pre_file"],
)
