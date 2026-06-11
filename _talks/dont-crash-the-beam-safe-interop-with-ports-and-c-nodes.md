---
tags:
  - interoperability
  - ports
  - c nodes

level: Intermediate
title: "Don't Crash the BEAM: Safe Interop with Ports and C Nodes"
speakers:
- _participants/riccardo-binetti.md
published: true

---
You've mastered the art of the NIF and squeezed every ounce of performance out of your code. But with great power comes great responsibility (and the occasional segfault that takes down your production node).

This talk explores how to run native code without risking the stability of your virtual machine.

We will start by looking at Ports, the simplest way to move dangerous code into a separate OS process. We'll cover the protocols for talking to standard input/output and how to ensure your external program doesn't turn into a zombie if the BEAM decides to restart.

Then we'll move on to the heavy artillery: C Nodes. We'll see how to use the `ei` library to make an external executable behave like an Erlang node. Did you know native code can connect to epmd, participate in the cluster and exchange messages just like a GenServer? We will demystify the setup required to make this happen and discuss the security implications.

Finally, we will break down the tradeoffs between them, comparing latency, complexity and fault tolerance, so you know exactly which tool to reach for when a NIF is just too risky.

**Key Takeaways:**

- Learn how to implement robust Ports that handle backpressure and lifecycle management
- Understand how to build a C Node that connects to your cluster
- Have a clear decision matrix for choosing between NIFs, Ports, and C Nodes based on latency and safety requirements

**Target Audience:**

- Elixir developers who need native performance but cannot afford VM crashes
- Engineers looking to integrate legacy C/C++ applications or heavy computational services into a BEAM architecture
