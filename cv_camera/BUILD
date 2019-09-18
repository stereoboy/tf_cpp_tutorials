#
# references
#  - https://github.com/tensorflow/tensorflow/issues/7288
#

load("//tensorflow:tensorflow.bzl", "tf_cc_binary")
tf_cc_binary(
    name = "viewer",
    srcs = glob([
         "*.cc",
         "*.h",
    ]),
    copts = [
              #"-z",
              #"-std=c++11",
        #"-Wl,--as-needed -lopencv_freetype",
    ],
    linkopts = [
        #"-lm",
        #"-Wl,--as-needed -lopencv_freetype",
        "-lopencv_video -lopencv_stereo -lopencv_structured_light -lopencv_rgbd -lopencv_viz -lopencv_text -lopencv_ximgproc -lopencv_calib3d -lopencv_features2d -lopencv_flann -lopencv_xobjdetect -lopencv_objdetect -lopencv_highgui -lopencv_videoio -lopencv_imgcodecs -lopencv_photo -lopencv_imgproc -lopencv_core",
    ],
    deps = [
        "//tensorflow/cc:cc_ops",
        "//tensorflow/cc:client_session",
        "//tensorflow/core:tensorflow",
    ],
)
