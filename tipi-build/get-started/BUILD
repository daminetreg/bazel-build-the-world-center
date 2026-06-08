load("@rules_cc//cc:defs.bzl", "cc_test")

cc_test(
    name = "get_started_test",
    srcs = ["test/main.cpp"],
    copts = ["-std=c++17"],
)

filegroup(
    name = "all_sources",
    srcs = [
        "CMakeLists.txt",
        "NOINSTALL_FIRST_STEPS.md",
        "README.md",
        "test/main.cpp",
        "environments/compiler/clang.cmake",
        "environments/flags/cxx17.cmake",
        "environments/linux.cmake",
        "environments/linux.container.lock",
        "environments/linux.pkr.js/linux.Dockerfile",
        "environments/linux.pkr.js/linux.pkr.js",
        ".github/workflows/ci.yaml",
        ".gitignore",
        ".tipi/deps",
    ],
    visibility = ["//visibility:public"],
)
