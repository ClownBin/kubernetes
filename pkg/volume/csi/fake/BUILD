load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "fake_client.go",
        "fake_closer.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/volume/csi/fake",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/container-storage-interface/spec/lib/go/csi/v0:go_default_library",
        "//vendor/google.golang.org/grpc:go_default_library",
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
    visibility = ["//visibility:public"],
)
