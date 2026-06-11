---
tags:
  - beam-languages
  - static-analysis
  - gleam

level: Intermediate
title: "Same Runtime, Different Language: Adapting SAFE for Gleam"
speakers:
- _participants/robert-fiko.md
published: true

---
This year, we dreamed big: let’s adapt SAFE (our static analysis security tool) for Gleam. It shouldn’t be too hard, we thought, since we already adapted it for Elixir. We were wrong.
Even though Erlang, Elixir, and Gleam all compile to the BEAM, the differences in their compilation pipelines challenged us in ways we didn’t expect. In this talk, I’ll tell the story of how we transitioned SAFE from Erlang and Elixir to Gleam, comparing how each language compiles to BEAM and where our first ideas broke.
We’ll look at how Erlang–Elixir interop differs from Gleam–Erlang interop, what that means for static analysis, and why using simple Erlang checks is not enough. Finally, I’ll show how security analysis for Gleam actually works with a live demo of SAFE in action.
By the end, attendees should understand what static analysis across BEAM languages taught us.

**Key Takeaways:**

- Same runtime does not mean same analysability
- Interop is not the same across the BEAM languages
- The devil is in the details, especially during compilation.

**Target Audience:**

- Gleam developers, tech leads
- Security engineers in Gleam teams
