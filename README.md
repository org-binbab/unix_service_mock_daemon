# Unix Mock Service Daemon (UMSD)An underlying script for a unix service simulate. Designed to track start/stop/reload actions in order to evaluate the operation of a wrapper or service management platform.## Usage    $ ./service_daemon.sh --help```Usage: service_daemon.sh OPTIONSDefault port: 1234Response format:  TEST_STRING START_TIME PARENT_PID START_PID START_USER RELOAD_COUNTERExample usage:
  ./service_daemon.sh &
  nc localhost 1234  >>> Soundslikefunonabun 1372658056 -1 86056 nobody 0Available options:  --fork              Fork and return immediately  --no-reload         Exit on reload (SIGHUP)  --port PORT         Listen on alternate port```## Development and Maintenance* Found a bug?* Need some help?* Have a suggestion?* Want to contribute?Please visit: [code.binbab.org](http://code.binbab.org)## Authors and License  * Author:: BinaryBabel OSS (<projects@binarybabel.org>)  * Copyright:: 2013 `sha1(OWNER) = df334a7237f10846a0ca302bd323e35ee1463931`  * License:: Apache License, Version 2.0----    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.