# ==================================================================================================
# Copyright 2011 Twitter, Inc.
# --------------------------------------------------------------------------------------------------
# Licensed to the Apache Software Foundation (ASF) under one or more contributor license
# agreements.  See the NOTICE file distributed with this work for additional information regarding
# copyright ownership.  The ASF licenses this file to you under the Apache License, Version 2.0
# (the "License"); you may not use this file except in compliance with the License.  You may
# obtain a copy of the License at
#
#  http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software distributed under the
# License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
# express or implied.  See the License for the specific language governing permissions and
# limitations under the License.
# ==================================================================================================

from pants import *

java_library(name = 'http',
  provides = artifact(
    org = 'com.twitter.common',
    name = 'net-http',
    repo = pants('build-support/commons/ivy:public'),
  ),
  dependencies = [
    pants('3rdparty:guava'),
    pants('3rdparty:guice'),
    pants('3rdparty:guice-servlet'),
    pants('3rdparty:jetty'),
    pants('3rdparty:jsr305'),
    pants('3rdparty:servlet-api'),
    pants('src/java/com/twitter/common/net/http/handlers:text'),
  ],
  sources = globs('*.java')
)