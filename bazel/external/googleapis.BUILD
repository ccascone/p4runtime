package(
    default_visibility = [ "//visibility:public" ],
)

load("@org_pubref_rules_protobuf//cpp:rules.bzl", "cpp_proto_library")
load("@org_pubref_rules_protobuf//python:rules.bzl", "py_proto_compile")
load("@org_pubref_rules_protobuf//java:rules.bzl", "java_proto_library")

cpp_proto_library(
    name = "status_proto_cc",
    protos = ["google/rpc/status.proto"],
    imports = ["external/com_google_protobuf/src/"],
    inputs = ["@com_google_protobuf//:well_known_protos"],
    with_grpc = False,
)

py_proto_compile(
    name = "status_proto_py",
    protos = ["google/rpc/status.proto"],
    imports = ["external/com_google_protobuf/src/"],
    inputs = ["@com_google_protobuf//:well_known_protos"],
    with_grpc = False,
)

java_proto_library(
    name = "status_proto_java",
    protos = ["google/rpc/status.proto"],
    imports = ["external/com_google_protobuf/src/"],
    inputs = ["@com_google_protobuf//:well_known_protos"],
    with_grpc = False,
)

proto_library(
    name = "google_rpc_status_proto",
    srcs = ["google/rpc/status.proto"],
    deps = ["@com_google_protobuf//:any_proto"],
)