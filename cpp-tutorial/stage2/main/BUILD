# 注释
# 构建命令: bazel build //main:hello-world
load("@rules_cc//cc:defs.bzl", "cc_binary", "cc_library")

cc_library(
    name = "hello-greet",
    srcs = ["hello-greet.cc"],
    hdrs = ["hello-greet.h"],
)

cc_binary(
    name = "hello-world",
    srcs = ["hello-world.cc"],
    # deps 用于声明依赖的库
    deps = [
        ":hello-greet",
    ],
)
