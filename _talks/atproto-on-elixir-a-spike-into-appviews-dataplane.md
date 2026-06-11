---
tags:
  - ATProto Bluesky RoaringBitmaps

level: Intermediate
title: "ATProto on Elixir: A Spike into AppView's DataPlane"
speakers:
- _participants/chris-beck.md
published: true

---
Twitter's decline has led to increased interest in alternatives, with Bluesky being a notable option.

The Bluesky team seeks to establish ATProto as an IETF internet standard for building social application infrastructure. Most of its components are open source, enabling self-hosting.

An exception is AppView's DataPlane. The open-source Node/Postgres implementation has scaling issues, while the closed-source V2 (Go and ScyllaDB) demands terabytes of RAM.

In February 2026, the EEF founded a project to build a DataPlane proof of concept in Elixir. Combining Elixir and Rust, we built a POC that outperforms the legacy DataPlane, scales to millions of users, and runs on a fraction of the resources the commercial implementation requires.

This talk introduces the Bluesky and ATProto landscape, shows where the DataPlane fits, and presents our results—including a live performance demonstration.

**Key Takeaways:**

- ## Architectural
- How ATProto and Bluesky are structured, and where the DataPlane sits within the AppView
- Why the DataPlane is the critical scaling bottleneck in a self-hosted Bluesky stack
- ## Technical / Elixir-specific
- How the BEAM's concurrency model maps onto the DataPlane's workload (high-fanout reads, fan-out feeds, etc.)
- Where Rust NIFs make sense as a complement to Elixir, and how to draw that boundary
- Concrete performance numbers: throughput, latency, and resource footprint versus both the Node/Postgres and Go/ScyllaDB implementations
- ## Practical
- That a resource-efficient, self-hostable DataPlane is viable—lowering the barrier to running independent AppViews
- Lessons learned and pitfalls from building it (data modeling, indexing strategy, what didn't work)
- The current state of the project and how to get involved / what's next

**Target Audience:**

- Beam engineers who are considering to build a social app
- People interested in digital independence
- People interested to get involved
