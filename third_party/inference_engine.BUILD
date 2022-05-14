# Description:
#   inference_engine libraries for NN on Linux

licenses(["notice"])  # BSD license

exports_files(["LICENSE"])


cc_library(
    name = "inference_engine",
    hdrs = glob([
        "include/**/*.h*",
        "include/*.h*",
    ]),
    includes = [
        "include/",
    ],
    linkopts = [
        "-L/opt/intel/openvino_2021/deployment_tools/inference_engine/lib/intel64",
        "-l:libinference_engine.so",
        "-l:libinference_engine_legacy.so",
        "-l:libinference_engine_transformations.so",
        "-l:libinference_engine_c_api.so",
    ],
    visibility = ["//visibility:public"],
)
