load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "config.go",
        "egress_selector.go",
    ],
    importmap = "k8s.io/cloud-provider-gcp/vendor/k8s.io/apiserver/pkg/server/egressselector",
    importpath = "k8s.io/apiserver/pkg/server/egressselector",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/google.golang.org/grpc:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/net:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/validation/field:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/apis/apiserver:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/apis/apiserver/install:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/apis/apiserver/v1beta1:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/server/egressselector/metrics:go_default_library",
        "//vendor/k8s.io/klog/v2:go_default_library",
        "//vendor/k8s.io/utils/path:go_default_library",
        "//vendor/k8s.io/utils/trace:go_default_library",
        "//vendor/sigs.k8s.io/apiserver-network-proxy/konnectivity-client/pkg/client:go_default_library",
        "//vendor/sigs.k8s.io/yaml:go_default_library",
    ],
)
