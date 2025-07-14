---
tags:
  - Simple
  - Practical
  - Composable

level: advanced
title: "Reactor Under the Hood: Building a Graph-Based Saga Orchestrator in Elixir"
speakers:
  - _participants/james-harton.md

---
Here's the thing - workflow engines sound complicated, but they don't have to be. I'll show you how Reactor uses a dead simple graph algorithm (find nodes with no dependencies, run them, remove them, repeat) to build something genuinely useful. We'll dig into how this basic approach, combined with OTP, gives you concurrent execution with concurrency limits, automatic retries, compensation when things go wrong (and they will), and the ability to compose workflows inside each other. You'll see how we made the simple cases easy without making the complex cases impossible.

**Key Takeaways:**

- How a basic graph traversal becomes a proper execution engine when you add OTP to the mix
- Managing shared concurrency pools so nested Reactors don't starve each other of resources
- Building compensation patterns that actually work when production decides to test your error handling
- Making APIs that don't make developers want to flip tables (harder than it sounds)

**Target Audience:**

- Elixir developers who want to understand advanced OTP patterns, folks building libraries, system architects
