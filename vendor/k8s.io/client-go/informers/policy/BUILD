load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["interface.go"],
    importmap = "k8s.io/cloud-provider-gcp/vendor/k8s.io/client-go/informers/policy",
    importpath = "k8s.io/client-go/informers/policy",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/k8s.io/client-go/informers/internalinterfaces:go_default_library",
        "//vendor/k8s.io/client-go/informers/policy/v1:go_default_library",
        "//vendor/k8s.io/client-go/informers/policy/v1beta1:go_default_library",
    ],
)
