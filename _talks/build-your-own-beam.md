---
tags:
  - beam
  - elixir
  - concurrency

level: Intermediate
title: "Build Your Own BEAM"
speakers:
- _participants/martin-janiczek.md
published: true

---
We'll build a toy single-threaded implementation of the BEAM virtual machine, based on "The BEAM Book" - the scheduler, the virtual machine and so on, and then run some example programs on it and visualize what it's doing under the hood.

**Key Takeaways:**

- How and when to use Erlang Doctor to speed up tracing/debugging.
- How to improve their own code to make it easier to debug and comprehend.

**Target Audience:**

- Erlang/Elixir engineers facing the reality - software with bugs, most of them difficult to find, especially if the system is complex
