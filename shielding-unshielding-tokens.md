# Shielding / Unshielding Tokens

In zk-SNARKs, a shielded address, also known as a "z-address," is a type of address that is used to protect the privacy of the user. The main difference between a shielded address and an unshielded address (also known as a "t-address") is that transactions to and from a shielded address are hidden on the blockchain, whereas transactions to and from an unshielded address are publicly visible.

In the context of Ethereum, a shielded address can be implemented using a smart contract called a "shield contract" that provides functions to deposit and withdraw ERC20 tokens. The deposit function, typically named "shield", takes an ERC20 token and sends it to the shield contract, where it is locked until the user decides to withdraw it. When the user wants to withdraw their tokens, they can call the withdraw function on the shield contract, which sends the tokens back to the user's unshielded address.
