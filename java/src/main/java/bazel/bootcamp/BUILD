java_binary(
    name = "HelloBazelBootcamp",
    srcs = ["HelloBazelBootcamp.java"],
    main_class = "bazel.bootcamp.HelloBazelBootcamp",
    deps = [],
)

java_binary(
    name = "JavaLoggingClient",
    srcs = ["JavaLoggingClient.java"],
    main_class = "bazel.bootcamp.JavaLoggingClient",
    deps = [
        ":JavaLoggingClientLibrary",
    ],
    visibility = ["//visibility:public"],
)

java_library(
    name = "logging_client_test_lib",
    srcs = ["JavaLoggingClientTest.java"],
    deps = [
        "@junit_junit//jar",
    ],
)

java_test(
    name = "logging_client_test",
    test_class = "bazel.bootcamp.JavaLoggingClientTest",
    runtime_deps = [
        ":logging_client_test_lib",
    ],
)

java_library(
    name = "JavaLoggingClientLibrary",
    srcs = ["JavaLoggingClientLibrary.java"],
    deps = [
        "//proto/logger:logger_java_proto",
        "//proto/logger:logger_java_grpc",
        "@io_grpc_grpc_java//core",
        "@io_grpc_grpc_java//netty",
    ],
)

java_library(
    name = "logging_client_library_test_lib",
    srcs = ["JavaLoggingClientLibraryTest.java"],
    deps = [
        ":JavaLoggingClientLibrary",
        "@junit_junit//jar",
    ],
)

java_test(
    name = "logging_client_library_test",
    test_class = "bazel.bootcamp.JavaLoggingClientLibraryTest",
    runtime_deps = [
        ":logging_client_library_test_lib",
    ],
)

# deps you may need for various targets

#    "@io_grpc_grpc_java//netty",
#    "@junit_junit//jar" - optional
