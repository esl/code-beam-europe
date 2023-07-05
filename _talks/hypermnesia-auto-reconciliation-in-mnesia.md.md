---
tags:	
- "Mnesia, CRDTs, Eventual Consistency"
level: Intermediate
title: 	"Hypermnesia: Auto Reconciliation in Mnesia"
speakers: 
- _participants/shuntian-liu.md

---
Mnesia is an embedded database for Erlang/OTP applications that offers outstanding performance thanks to its tight integration with Erlang. However, its lack of conflict resolution after network partitions is a notable limitation that demands manual restart by developers to reconcile replicas.
In this talk, I will discuss eventual consistency and CRDTs to achieve automatic conflict resolution within Mnesia. I will introduce Hypermnesia, an extension to Mnesia featuring a new access context async_ec that streamlines replica reconciliation after a partition.
Hypermnesia is also designed with minimising overhead and out-of-box usage in mind. In the talk, I will present benchmarking results, and demonstrate practical examples of using Hypermnesia.
This project is a collaboration between the University of Cambridge and Erlang Solutions.

**Key Takeaways:**
- You will learn
* what problems Mnesia has and why they are important
* how to achieve automatic conflict resolution in Mnesia
* how eventual consistency and CRDTs can help us
* overhead of eventual consistency in Mnesia
* Example usage of the new API

**Target Audience:**
- Mnesia users, CRDTs developers, and people with a general interest in distributed system consistency.