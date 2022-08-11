load("@rules_cc//cc:defs.bzl", "cc_library")

cc_library(
    name = "hello-time",
    srcs = ["hello-time.cc"],
    hdrs = ["hello-time.h"],
    # visibility 用来设置可见性
    # 默认情况下，目标仅对同一 BUILD 文件中的其他目标可见
    # 这句声明表示让 //lib:hello-time 对 main/BUILD 中的其他目标可见
    visibility = ["//main:__pkg__"],
)
