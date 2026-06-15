---
experience:
- Intermediate
title: "Gnome Village: Understanding the BEAM Through Processes, Flows, and Runtime Behaviour"
type: tutorial
event_date: 20 Oct 2026
venue: TBC
trainers:
- _participants/erik-stenman.md
- _participants/mans-af-klercker.md
---
The BEAM is often introduced through Erlang or Elixir syntax, OTP behaviours, and supervision trees. Those are useful entry points, but they do not fully explain why BEAM systems behave the way they do in production.

This hands-on training uses the Gnome Village model to make BEAM internals and runtime architecture easier to reason about. Each gnome represents a process with its own heap, mailbox, reductions, failure boundary, and role in a larger system. Villages represent supervision structures and domains. Roads represent message flows. Gatekeepers, workers, coordinators, routers, caches, boundaries, and observers represent recurring process archetypes in real systems.

Participants will build and inspect small BEAM systems while connecting OTP design decisions to runtime behaviour. We will look at process creation, message passing, scheduling, garbage collection, supervision, bottlenecks, mailbox growth, back pressure, and failure containment. The aim is to move beyond "use GenServer here" and toward a practical model for understanding how concurrent BEAM systems actually run.

This course is for developers who want to understand the BEAM deeply enough to design systems that remain observable, maintainable, and resilient under load.

**Duration:**
* 8 hours

**Tutorial objectives:**
The training helps Erlang and Elixir developers build a practical mental model of how BEAM systems behave at runtime.

Participants will learn to connect OTP design choices to concrete runtime effects: process isolation, message passing, scheduling, mailboxes, supervision, garbage collection, bottlenecks, and failure propagation. They will use the Gnome Village model to reason about processes, flows, domains, and recurring process archetypes such as workers, gatekeepers, coordinators, routers, caches, boundaries, and observers.

The goal is that participants leave able to inspect an existing BEAM system, describe how work moves through it, identify where ownership and load accumulate, and make better design decisions when building or debugging concurrent systems.

**Target audience:**
* Erlang and Elixir developers who have used OTP and want a deeper understanding of BEAM runtime behaviour. The course also fits architects and senior engineers who design or operate BEAM systems in production.

**Prerequisites:**
* Participants should be comfortable reading basic Erlang or Elixir code. Prior experience with GenServer, supervision trees, or OTP applications is helpful. Deep BEAM knowledge is not required.
