package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)
load("//defs:version.bzl", "version_x_defs")

go_library(
    name = "go_default_library",
    srcs = ["provider.go"],
    importpath = "k8s.io/cloud-provider-gcp/cmd/auth-provider-gcp/provider",
    deps = [
        "//pkg/credentialconfig:go_default_library",
        "//pkg/gcpcredential:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/kubelet/pkg/apis/credentialprovider/v1alpha1:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["provider_test.go"],
    embed = [":go_default_library"],
    deps = [
        "//pkg/gcpcredential:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/net:go_default_library",
        "//vendor/k8s.io/kubelet/pkg/apis/credentialprovider/v1alpha1:go_default_library",
    ],
)
