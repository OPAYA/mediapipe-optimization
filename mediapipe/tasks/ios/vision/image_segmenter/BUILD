# Copyright 2023 The MediaPipe Authors.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
package(default_visibility = ["//mediapipe/tasks:internal"])

licenses(["notice"])

objc_library(
    name = "MPPImageSegmenterResult",
    srcs = ["sources/MPPImageSegmenterResult.m"],
    hdrs = ["sources/MPPImageSegmenterResult.h"],
    deps = [
        "//mediapipe/tasks/ios/core:MPPTaskResult",
        "//mediapipe/tasks/ios/vision/core:MPPMask",
    ],
)

objc_library(
    name = "MPPImageSegmenterOptions",
    srcs = ["sources/MPPImageSegmenterOptions.m"],
    hdrs = ["sources/MPPImageSegmenterOptions.h"],
    deps = [
        ":MPPImageSegmenterResult",
        "//mediapipe/tasks/ios/core:MPPTaskOptions",
        "//mediapipe/tasks/ios/vision/core:MPPRunningMode",
    ],
)

objc_library(
    name = "MPPImageSegmenter",
    hdrs = ["sources/MPPImageSegmenterOptions.h"],
    deps = [
        ":MPPImageSegmenterOptions",
        ":MPPImageSegmenterResult",
        "//mediapipe/tasks/ios/vision/core:MPPImage",
    ],
)
