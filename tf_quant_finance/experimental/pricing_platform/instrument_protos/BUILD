# Protos for portfolio and market data representation

load("@protobuf//bazel:py_proto_library.bzl", "py_proto_library")
load("@protobuf//bazel:proto_library.bzl", "proto_library")


package(
    default_visibility = ["//visibility:public"],
    licenses = ["notice"],
)

py_library(
    name = "instrument_protos",
    srcs = ["__init__.py"],
    deps = [
        ":instruments_py_pb2",
    ],
)

proto_library(
    name = "instruments_proto",
    srcs = [
        "all_instruments.proto",
        "american_equity_option.proto",
        "forward_rate_agreement.proto",
        "interest_rate_swap.proto",
        "swaption.proto",
    ],
    deps = [
        ":business_days_py_pb2",
        ":currencies_py_pb2",
        ":date_py_pb2",
        ":daycount_conventions_py_pb2",
        ":decimal_py_pb2",
        ":metadata_py_pb2",
        ":period_py_pb2",
        ":rate_indices_py_pb2",
    ],
)

py_proto_library(
    name = "instruments_py_pb2",
    visibility = ["//visibility:public"],
    deps = [":instruments_proto"],
)

proto_library(
    name = "daycount_conventions_proto",
    srcs = ["daycount_conventions.proto"],
)

py_proto_library(
    name = "daycount_conventions_py_pb2",
    visibility = ["//visibility:public"],
    deps = [":daycount_conventions_proto"],
)

proto_library(
    name = "decimal_proto",
    srcs = ["decimal.proto"],
)

py_proto_library(
    name = "decimal_py_pb2",
    visibility = ["//visibility:public"],
    deps = [":decimal_proto"],
)

proto_library(
    name = "date_proto",
    srcs = ["date.proto"],
)

py_proto_library(
    name = "date_py_pb2",
    visibility = ["//visibility:public"],
    deps = [":date_proto"],
)

proto_library(
    name = "currencies_proto",
    srcs = ["currencies.proto"],
)

py_proto_library(
    name = "currencies_py_pb2",
    visibility = ["//visibility:public"],
    deps = [":currencies_proto"],
)

proto_library(
    name = "metadata_proto",
    srcs = ["metadata.proto"],
)

py_proto_library(
    name = "metadata_py_pb2",
    visibility = ["//visibility:public"],
    deps = [":metadata_proto"],
)

proto_library(
    name = "period_proto",
    srcs = ["period.proto"],
)

py_proto_library(
    name = "period_py_pb2",
    visibility = ["//visibility:public"],
    deps = [":period_proto"],
)

proto_library(
    name = "rate_indices_proto",
    srcs = ["rate_indices.proto"],
)

py_proto_library(
    name = "rate_indices_py_pb2",
    visibility = ["//visibility:public"],
    deps = [":rate_indices_proto"],
)

proto_library(
    name = "business_days_proto",
    srcs = ["business_days.proto"],
)

py_proto_library(
    name = "business_days_py_pb2",
    visibility = ["//visibility:public"],
    deps = [":business_days_proto"],
)
