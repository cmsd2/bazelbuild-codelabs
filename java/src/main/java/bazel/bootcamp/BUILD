java_binary(
    name = "logging_client",
    srcs = ["JavaLoggingClient.java"],
    main_class = "bazel.bootcamp.JavaLoggingClient",
    deps = [
        ":logging_client_lib",
    ],
)

java_library(
    name = "logging_client_lib",
    srcs = ["JavaLoggingClientLibrary.java"],
    deps = [
        "//proto/logger:logger_java_proto",
        "//proto/logger:logger_java_grpc",
        "@io_grpc_grpc_java//core",
        "@io_grpc_grpc_java//netty",
    ],
)

# deps you may need for various targets

#    "@io_grpc_grpc_java//netty",
#    "@junit_junit//jar" - optional
