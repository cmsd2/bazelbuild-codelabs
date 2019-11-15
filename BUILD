package(default_visibility = ["//visibility:public"])

alias(
    name = "tsconfig.json",
    actual = "//typescript:tsconfig.json",
)

load("@bazel_gazelle//:def.bzl", "gazelle")

# gazelle:prefix github.com/bazelbuild/codelabs
# gazelle:exclude typescript/node_modules
gazelle(
    name = "gazelle",
)
