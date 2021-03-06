#
# Copyright 2018 ZetaSQL Authors
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#

licenses(["notice"])  # Apache v2.0

package(default_visibility = ["//:__subpackages__"])

cc_library(
    name = "status_matchers",
    testonly = 1,
    srcs = ["status_matchers.cc"],
    hdrs = ["status_matchers.h"],
    copts = [
        "-Wno-pessimizing-move",
        "-Wno-return-type",
        "-Wno-sign-compare",
        "-Wno-switch",
        "-Wno-unused-but-set-parameter",
        "-Wno-unused-function",
    ],
    deps = [
        "@com_google_googletest//:gtest",
        "//zetasql/base:source_location",
        "//zetasql/base:status",
        "@com_google_absl//absl/status",
        "@com_google_absl//absl/strings",
    ],
)

cc_test(
    name = "status_matchers_test",
    size = "small",
    srcs = ["status_matchers_test.cc"],
    copts = [
        "-Wno-pessimizing-move",
        "-Wno-return-type",
        "-Wno-sign-compare",
        "-Wno-switch",
        "-Wno-unused-but-set-parameter",
        "-Wno-unused-function",
    ],
    deps = [
        ":status_matchers",
        "@com_google_googletest//:gtest_main",
        "@com_google_googletest//:gtest",
        "//zetasql/base:status",
        "@com_google_absl//absl/status",
    ],
)
