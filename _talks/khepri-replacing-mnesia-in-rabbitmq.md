---
tags:	
- database, raft, mnesia
level: Introductory and overview
title: 	"Khepri: Replacing Mnesia in RabbitMQ"
speakers:
- _participants/michael-davis.md

---
Khepri is a tree-like, replicated database library from the RabbitMQ team using the Raft distributed consensus algorithm. Khepri aims to replace Mnesia for persistent and replicated metadata storage within RabbitMQ. This talk touches on why and how the Rabbit team chose to create Khepri, some basic usage examples and implementation details, recent large changes in Khepri, and updates on Khepri's progress into the RabbitMQ codebase:
* A new feature called "projections" allows us to match or beat mnesia's read speed in many cases.
* We've overhauled the API to be more ergonomic and also made it friendlier for Elixir.
* We plan on landing the Khepri branch in the next minor release under a feature flag!

**Key Takeaways:**
- The RabbitMQ team is working on replacing Mnesia with Khepri, our tree-like, replicated database library based on the Raft distributed consensus algorithm. You'll hear about why we want to move away from Mnesia, previous attempts we made, and our recent and promising progress. I'll introduce you to Khepri and we'll discuss the challenges we've faced and the changes we've made to match Mnesia's speed and improve ergonomics.

**Target audience:**
- Anyone interested in distributed computing on the BEAM, replication and databases.
- Users or those interested in RabbitMQ.
- Those curious about alternatives to Mnesia.