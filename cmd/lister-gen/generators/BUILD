package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "expansion.go",
        "lister.go",
        "tags.go",
    ],
    importpath = "github.com/modeljetpublic/k8s-code-generator-r18/cmd/lister-gen/generators",
    deps = [
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/github.com/modeljetpublic/k8s-code-generator-r18/cmd/client-gen/generators/util:go_default_library",
        "//vendor/github.com/modeljetpublic/k8s-code-generator-r18/cmd/client-gen/types:go_default_library",
        "//vendor/k8s.io/gengo/args:go_default_library",
        "//vendor/k8s.io/gengo/generator:go_default_library",
        "//vendor/k8s.io/gengo/namer:go_default_library",
        "//vendor/k8s.io/gengo/types:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)
