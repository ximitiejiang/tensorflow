licenses(["notice"])  # Apache 2.0

load("//tensorflow:tensorflow.bzl", "py_test")

filegroup(
    name = "all_files",
    srcs = glob(
        ["**/*"],
        exclude = [
            "**/METADATA",
            "**/OWNERS",
        ],
    ),
    visibility = ["//tensorflow:__subpackages__"],
)

py_library(
    name = "autograph",
    srcs = [
        "__init__.py",
    ],
    srcs_version = "PY2AND3",
    visibility = ["//visibility:public"],
    deps = [
        "//tensorflow/contrib/autograph/impl",
        "//tensorflow/contrib/autograph/lang",
        "//tensorflow/contrib/autograph/pyct",
        "//tensorflow/contrib/autograph/utils",
        "//tensorflow/python:util",
    ],
)
