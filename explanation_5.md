The BlockChain example was implemented using a regular linked list, with the head starting on the first block, and each block having a next pointer to the most recent one. Each block is assigned the previous block hash and generates a unique hash based on timestamp, data, and the previous hash. Using the previous hash as part of the new hash helps to prevent tampering of older blocks, as new hashes need to be generated.

This basic example doesn't take into account the proof of work or the more complex bitcoin protocol on the network. The time complexity for adding a new block is O(1). No delete operation is needed since we want to keep all the transactions history intact.
Space complexity is O(n), where n is the number of blocks.
