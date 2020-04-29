Hash break application via brute force
using multi-processes and distributed processing
with rabbitMQ, developed for the subject of Distributed Systems at PUC-GO.

To search for a hash via the command line, you need to run the following:
- minionRPC.py
- DataServer.py
- at least one instance of minionWorker.py on a machine with access to the host's ip where dDataServer.py is running

to search for a hash via web search (GET method /search/?hash=""), you need to run the following:
- CliAndDataServer.py
- at least one instance of minionWorker.py on a machine with access to the host's ip where CliAndDataServer.py is running

CliAndDataServer.py to DataServer.py
- In order for DataServers to serve files, it is necessary to execute the first time passing the arguments to create the word lists. For this, it is necessary to download an initial word list and inform the path to the data server through arguments so that it can divide it into smaller lists and serve the minions.
- The arguments for starting word lists are: -initF true -file "pathToWordlist.txt"
