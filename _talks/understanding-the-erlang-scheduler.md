---
tags: 
  - beam

level: Intermediate
title: "BEAM Internals: Understanding the Erlang Scheduler"
speakers: 
  - _participants/sanne-kalkman.md

---
Until recently, I took the magic of the BEAM for granted. Like many of us, I spawned processes, passed messages and happily used concurrency without much thought about how any of it really worked. While there is so much more to learn than fits in any one talk, this one aims to give an overview of the Erlang Scheduler and how it allows us write concurrent software without having to think about the hard parts.

**Key Takeaways:**

- An accessible introduction into an important but  -- to many developers -- mysterious part of the BEAM.

**Target Audience:**

- Anyone who uses Elixir or Erlang, but hasn't yet dug deeply into the BEAM internals.
