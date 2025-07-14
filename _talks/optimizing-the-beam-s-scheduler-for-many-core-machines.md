---
tags: 
  - scheduler
  - concurrency
  - optimisation

level: Advanced
title: "Optimizing the BEAM's Scheduler for Many-Core Machines"
speakers: 
  - _participants/robin-morisset.md

---
The BEAM is famous for supporting many lightweight processes. But the scheduler responsible for deciding which of these processes should execute on which core at which time was designed at a time when most servers only had a few cores, and can suffer from severe lock contention issues when used on many-core machines (100+ cores).
In this talk I'll explain the main ideas behind how the BEAM's scheduler works, how to discover and investigate lock-contention issues, and then explain some recent changes that mitigated these issues for the BEAM's scheduler.

**Key Takeaways:**

- The general design of the BEAM's scheduler (task-stealing, periodic rebalancing with immigration/emigration between runqueues)
- How to use lock-counting and interpret its results
- If you have performance issues on large servers, upgrade to the latest OTP for a large improvement

**Target Audience:**

- Anyone curious about the BEAM's internals, anyone struggling to improve the scalability of their Erlang/Elixir application on a many-core server.
