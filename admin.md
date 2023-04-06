# How can we send commands ("SLEEP", "RESTART", "ARE-YOU-THERE", etc) to individual nodes in the network, rather than treat them as pass-through intermediaries?

  I think again we should have a way that each node in the network should have a unique indentifier, which should be included in the header of each card that it receives. This should allow the sender to target specific nodes with commands. And then when a node receives a card with a command, it should recongnize the command by sending a response card back to the sender.
