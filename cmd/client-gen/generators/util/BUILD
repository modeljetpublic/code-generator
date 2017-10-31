package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["tags_test.go"],
    importpath = "github.com/modeljetpublic/k8s-code-generator-r18/cmd/client-gen/generators/util",
    library = ":go_default_library",
)

go_library(
    name = "go_default_library",
    srcs = ["tags.go"],
    importpath = "github.com/modeljetpublic/k8s-code-generator-r18/cmd/client-gen/generators/util",
    deps = ["//vendor/k8s.io/gengo/types:go_default_library"],
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
