load("@rules_java//java:defs.bzl", "java_library", "java_binary", "java_test")

package(default_visibility = ["//visibility:public"]) 

filegroup(
    name = "all_sources",
    srcs = glob([
        "**/*.h",
        "**/*.hh",
        "**/*.hpp",
        "**/*.c",
        "**/*.cc",
        "**/*.cpp",
        "**/*.cxx",
        "**/*.java",
        "**/*.lean",
        "**/*.sh",
        "**/*.bat",
        "**/*.template",
        "*.md",
        "*.txt",
    ]),
)

java_library(
    name = "ryu_java",
    srcs = glob(["src/main/java/**/*.java"]),
)

java_library(
    name = "ryu_java_tests_lib",
    srcs = glob(["src/test/java/**/*.java"]),
    deps = [":ryu_java"],
)

java_test(
    name = "ryu_java_tests",
    srcs = ["src/test/java/info/adams/ryu/AllTests.java"],
    deps = [":ryu_java"],
)

java_binary(
    name = "ryu_benchmark_java",
    srcs = ["src/main/java/info/adams/ryu/benchmark/BenchmarkMain.java"],
    main_class = "info.adams.ryu.benchmark.BenchmarkMain",
    deps = [":ryu_java"],
)
