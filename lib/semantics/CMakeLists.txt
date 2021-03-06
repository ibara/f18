# Copyright (c) 2018, NVIDIA CORPORATION.  All rights reserved.
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


add_library(FortranSemantics
  attr.cc
  canonicalize-do.cc
  expression.cc
  mod-file.cc
  resolve-labels.cc
  resolve-names.cc
  rewrite-parse-tree.cc
  scope.cc
  semantics.cc
  symbol.cc
  type.cc
  unparse-with-symbols.cc
)

target_link_libraries(FortranSemantics
  FortranCommon
  clangBasic
)
