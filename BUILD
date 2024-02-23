load("@rules_go//go:def.bzl", "go_binary", "go_library")
load("@gazelle//:def.bzl", "gazelle")

gazelle(name = "gazelle")

go_library(
    name = "sdkversionrepro_lib",
    srcs = ["main.go"],
    importpath = "github.com/mkmik/sdkversionrepro",
    visibility = ["//visibility:private"],
)

go_binary(
    name = "sdkversionrepro",
    embed = [":sdkversionrepro_lib"],
    visibility = ["//visibility:public"],
)
