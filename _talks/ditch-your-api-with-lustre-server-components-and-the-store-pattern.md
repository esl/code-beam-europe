---
tags:
  - ditch your api

level: Intermediate
title: "Ditch Your API with Lustre Server Components and the Store Pattern"
speakers:
- _participants/hayleigh-thompson.md
published: true

---
Full stack apps need a way for the client and server to talk to one another: a REST API, gRPC, or something else. Solutions like LiveView sidestep this problem by moving the render logic to the server – eliminating the "client" half of the equation entirely – but what about scenarios where you *want* code running clientside?

Lustre's server components bring LiveView-like functionality to Gleam applications allowing client events to be handled in realtime on the server, but they also allow the inverse with the server able to provide data to client-rendered children.

In this talk we'll look at how to leverage this functionality through the "store pattern," and see how we can eliminate the traditional API layer entirely.

**Key Takeaways:**

- Audience members will gain a better understanding of how Lustre's server components work, how they differ - both technically and philosophically - from Phoenix LiveView's, and how to get the most out of them.

**Target Audience:**

- BEAMers that want or need to write client code but want to side-step JavaScript, npm, package.json, ...
- Anyone that's struggled with full-stack app development and architecting the API layer.
