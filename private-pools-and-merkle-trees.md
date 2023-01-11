# Private pools and Merkle trees

Private pools and Merkle trees are related concepts used in zk-SNARKs for privacy preservation.

A private pool is a set of zk-SNARKs proofs that are combined together to form a larger proof. This can be done to improve privacy by hiding the relationship between different proofs, since the larger proof only reveals the overall balance of the pool, not the individual proofs.

A Merkle tree is a data structure used to efficiently prove the inclusion of a specific piece of data in a larger set of data, without revealing the entire set. In the context of private pools, a Merkle tree can be used to prove that a specific zk-SNARK proof is included in the pool, without revealing the contents of the entire pool.

Here is an example of how a Merkle tree can be used to implement a private pool:

* A Merkle tree is constructed from the leaves, which are the individual zk-SNARK proofs in the pool.
* The tree is constructed by repeatedly hashing pairs of child nodes together to form the parent node, until only the root of the tree remains.
* The root of the Merkle tree is publicly available and can be used to prove the inclusion of a specific zk-SNARK proof in the pool, without revealing the contents of the entire pool.

In the context of Ethereum, a Merkle Tree can be used to implement a ZK Rollup, which is a layer 2 scaling solution for zk-SNARKs. It allows to bundle multiple transactions into one zk-SNARK, effectively reducing the amount of data that need to be stored on-chain and thus reducing the gas cost of executing smart contract, while preserving privacy.
