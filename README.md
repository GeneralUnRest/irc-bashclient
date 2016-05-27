IRC botclient - Bash
====================

Depends on ncat.

Usage
-----

	./ircbot.sh -n nickname [-s server] [-p port] [-t] [-q] [-j]
	  -n --nick    user's nickname
	  -s --server  the server to connect to (default, rizon)
	  -p --port    port number to use (default, 6667)
	  -t --tls     enable tls connection (default, off)
		 --ssl     same as -t
	  -q --quiet   remove error and motd messages
	  -j --hide-joins

Once in, the bot/client has the following commands available to them:

	:j #chan         - join a channel
	:l #chan [msg]   - leave a channel
	:m #chan message - send message to channel
	:r anything      - send raw irc command
	:q [msg]         - quit

All commands start with a colon (:) and the arguments.
All the commands that take multiline arguments alreaady have the colon prepended to them, except for raw commads.

Licence
-------

Copyright 2016 prussian <generalunrest@airmail.cc>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

  <http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
