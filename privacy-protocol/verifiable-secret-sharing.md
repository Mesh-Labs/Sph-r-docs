# Verifiable secret sharing

A distinguished player who wishes to share the secret is referred to as the dealer in a VSS protocol. The protocol is divided into two phases: sharing and reconstruction.

Sharing begins with the dealer holding secret as input and each participant holding an individual random input. The sharing phase may be divided into numerous rounds. Each round, each player can privately message other players as well as broadcast a message. A player's message is determined by its input, random input, and messages received from other players in previous rounds.

{% hint style="info" %}
When you have an accident, your family members can manage your key.
{% endhint %}

Reconstruction: During this phase, each player submits their complete perspective from the sharing phase, and a reconstruction function is applied and the protocol's output is used. Oded Goldreich defines VSS as a safe multi-party protocol for computing the randomized functionality associated with some (non-verifiable) secret sharing method. This definition is more powerful than the others and is highly useful in the context of broad secure multi-party computation.

Secure multiparty computation requires verifiable secret sharing. Making hidden input shares and manipulating those shares to compute some function is the typical method for multiparty computation. The secret sharing system needs to be verifiable in order to manage "active" adversaries, or attackers that corrupt nodes and subsequently cause them to diverge from the protocol.
