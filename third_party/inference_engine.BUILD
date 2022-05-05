# Description:
#   inference_engine libraries for NN on Linux

licenses(["notice"])  # BSD license

exports_files(["LICENSE"])


cc_library(
    name = "inference_engine",
    hdrs = glob([
        "include/opencv4/opencv2/**/*.h*",
    ]),
    includes = [
        "include/opencv4/",
    ],
    linkopts = [
        "-L/usr/local/lib",
        "-l:libopencv_core.so",
        "-l:libopencv_calib3d.so",
    ],
    visibility = ["//visibility:public"],
)
