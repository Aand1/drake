# -*- python -*-
# This file contains rules for Bazel; see drake/doc/bazel.rst.

load("//tools:drake.bzl", "drake_cc_library")
load("//tools:lint.bzl", "add_lint_tests")

package(default_visibility = ["//visibility:public"])

drake_cc_library(
    name = "test_utilities",
    testonly = 1,
    srcs = [],
    hdrs = [],
    deps = [
        ":my_vector",
        ":pack_value",
        ":scalar_conversion",
    ],
)

drake_cc_library(
    name = "pack_value",
    testonly = 1,
    srcs = [],
    hdrs = ["pack_value.h"],
    deps = [
        "//drake/systems/framework:value",
    ],
)

drake_cc_library(
    name = "my_vector",
    testonly = 1,
    srcs = [],
    hdrs = ["my_vector.h"],
    deps = [
        "//drake/common:essential",
        "//drake/systems/framework:vector",
    ],
)

drake_cc_library(
    name = "scalar_conversion",
    testonly = 1,
    srcs = [],
    hdrs = ["scalar_conversion.h"],
    deps = [
        "//drake/common/test_utilities:is_dynamic_castable",
    ],
)

add_lint_tests()
