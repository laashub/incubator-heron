package(default_visibility = ["//visibility:public"])

pex_library(
    name = "executor-py",
    srcs = ["heron_executor.py"],
    deps = [
        "//heron/statemgrs/src/python:statemgr-py",
        "//heron/common/src/python:common-py",
    ],
    reqs = ["PyYAML==3.13"],
)

pex_binary(
    name = "heron-executor",
    srcs = ["heron_executor.py"],
    deps = [
        ":executor-py",
    ],
)
