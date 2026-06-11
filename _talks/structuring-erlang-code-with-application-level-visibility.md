---
tags:
  - Erlang
  - Boundaries
  - Maintainability

level: Intermediate
title: "Structuring Erlang Code with Application-Level Visibility"
speakers:
- _participants/erik-stenman.md
published: true

---
Erlang has strong module boundaries and explicit exports. In larger systems, that gives us a useful foundation, but it leaves one important question mostly to convention: which exported functions are part of the public API, and which ones are only meant to be used inside a local subsystem or application?

This talk presents the motivation behind a proposal for application-level export visibility in Erlang.

The problem is familiar in many mature Erlang systems. As codebases grow, internal helper APIs become exported because several modules need them. Over time, those exports become accidental APIs. Other parts of the system start depending on them, refactoring becomes harder, and the boundary between supported interface and implementation detail becomes vague.

The proposal explores how Erlang could express a middle ground between private functions and fully public exports. The goal is to make intended visibility explicit, help tools detect boundary violations, and give maintainers a clearer way to evolve large systems.

The talk will cover the problem, the proposed semantics, examples from real code, and the design trade-offs raised by the community discussion.

**Key Takeaways:**

- The audience will learn how accidental APIs appear in Erlang systems, why module-level export alone does not always express the intended boundary, and how application-level visibility could help maintainers evolve large systems with clearer interfaces and better tool support.

**Target Audience:**

- Erlang developers, library maintainers, OTP contributors, and teams working with larger Erlang codebases.
