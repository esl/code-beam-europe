---
tags:
  - static type checks
level: Intermediate
title: "Same same but different: Static type checkers for Erlang"
speakers:
- _participants/annette-bieniusa.md
- _participants/albert-schimpf.md
published: false
---
Though Erlang’s type annotations were originally intended for documentation purposes, static analysis tools soon utilized them for semantic checks. However, due to a need for more semantic agreement on Erlang’s type annotations, their results differ in ways that can be challenging for users to interpret. In our session, we cross-compare four state-of-the-art tools (Dialyzer, Gradualizer, eqWAlizer, etylizer) regarding their expressivity and performance. Their unified test suites provide a good starting point to understand their respective capabilities and limitations. Insights into the underlying approaches can help Erlang developers make an educated choice which analysis tool to use for their projects and how to interpret the result of a type check.

**Key Takeaways:**
- What are best practices for type annotations in Erlang?
- What gurantees do the different available type checkers give me?
- I got a type error - what now?
