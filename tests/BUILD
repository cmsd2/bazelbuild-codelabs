sh_test(
    name = "logging_integration_test",
    size = "small",
    srcs = ["integrationtest.sh"],
    data = [
        "//go/cmd/server:go-server",
        "//java/src/main/java/bazel/bootcamp:JavaLoggingClient",
    ],
    tags = ["exclusive"],
)
