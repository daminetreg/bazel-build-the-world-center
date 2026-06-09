filegroup(
    name = "all_srcs",
    srcs = glob([
        "**/*.cpp",
        "**/*.cc",
        "**/*.c",
        "**/*.h",
        "**/*.hpp",
        "**/*.ipp",
        "**/*.inc",
        "**/*.qbk",
        "**/*.jam",
        "**/*.cmake",
    ]),
    visibility = ["//visibility:public"],
)

cc_library(
    name = "phoenix_headers",
    hdrs = glob([
        "include/**/*.hpp",
        "include/**/*.h",
        "include/**/*.ipp",
    ]),
    includes = ["include"],
    visibility = ["//visibility:public"],
)
