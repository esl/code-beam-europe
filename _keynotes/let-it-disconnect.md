---
title: "Let It Disconnect: A Local-First Future"
speakers:
- _participants/brooklyn-zelenka.md

---
"Let it crash" was never really about crashing — it was about designing systems that assume failure and keep working anyway. Local-first software takes the same view about the network, service providers, and open source: assume disconnection, variable latency, service EOLs, and forks to design for convergence and user agency rather than coordination and lock-in.

We'll trace how the BEAM's core ideas — like shared-nothing architectures, supervision, and state on top of pure data — map directly on to local-first: CRDTs for conflict-free sync, capabilities for decentralised auth, and peer-to-peer protocols that work without a server in the loop. Less a new paradigm than the distribution model Erlang always implied, finally extended past the data center to each device directly.
