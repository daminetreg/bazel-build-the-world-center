load("@rules_cc//cc:defs.bzl", "cc_library", "cc_test")

package(default_visibility = ["//visibility:public"]) 

# Header-only Boost.Fusion library
cc_library(
    name = "fusion_headers",
    hdrs = glob([
        "include/**/*.hpp",
        "include/**/*.h",
    ]),
    includes = ["include"],
)

# Example binaries
cc_binary(
    name = "example_cookbook_do_the_bind",
    srcs = ["example/cookbook/do_the_bind.cpp"],
    deps = [":fusion_headers"],
)

cc_binary(
    name = "example_cookbook_fill_em_up",
    srcs = ["example/cookbook/fill_em_up.cpp"],
    deps = [":fusion_headers"],
)

cc_binary(
    name = "example_extension_test_example",
    srcs = ["example/extension/test_example.cpp"],
    deps = [":fusion_headers"],
)

cc_binary(
    name = "example_extension_triple",
    srcs = ["example/extension/triple.cpp"],
    deps = [":fusion_headers"],
)

cc_binary(
    name = "example_performance_accumulate",
    srcs = ["example/performance/accumulate.cpp"],
    deps = [":fusion_headers"],
)

cc_binary(
    name = "example_performance_functional",
    srcs = ["example/performance/functional.cpp"],
    deps = [":fusion_headers"],
)

cc_binary(
    name = "example_performance_inner_product",
    srcs = ["example/performance/inner_product.cpp"],
    deps = [":fusion_headers"],
)

cc_binary(
    name = "example_performance_inner_product2",
    srcs = ["example/performance/inner_product2.cpp"],
    deps = [":fusion_headers"],
)

cc_binary(
    name = "example_performance_sequence_efficiency",
    srcs = ["example/performance/sequence_efficiency.cpp"],
    deps = [":fusion_headers"],
)

cc_binary(
    name = "example_performance_zip_efficiency",
    srcs = ["example/performance/zip_efficiency.cpp"],
    deps = [":fusion_headers"],
)

filegroup(
    name = "all_source_files",
    srcs = glob([
        "**/*.cpp",
        "**/*.hpp",
        "**/*.h",
        "**/*.ipp",
        "**/*.qbk",
        "**/*.txt",
    ]),
)
