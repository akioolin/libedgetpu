# Copyright 2019 Google LLC
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

# Description:
#  Register access related functionality.

package(default_visibility = ["//visibility:public"])

licenses(["notice"])

cc_library(
    name = "registers",
    srcs = ["registers.cc"],
    hdrs = ["registers.h"],
    deps = ["//port"],
)

cc_library(
    name = "socket_registers",
    srcs = ["socket_registers.cc"],
    hdrs = ["socket_registers.h"],
    deps = [
        ":registers",
        "//port",
        "//port:std_mutex_lock",
        "//port:thread_annotations",
    ],
)
