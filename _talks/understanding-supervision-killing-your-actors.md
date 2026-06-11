---
tags:
  - supervision
  - gleam

level: Intermediate
title: "Understanding Supervision: Killing Your Actors"
speakers:
- _participants/kero-van-gelder.md
published: true

---
Supervisors have your back, but that is just part of the story. 

An actor that crashes is usually resurrected. Yet, some other process may try to interact with it while it is not yet alive. What happens next? One crash may cause another, which causes another - that is not what you had imagined!

We are going to slow down the interactions, kill some actors and observe the fallout.

We will approach this from the typed Gleam supervisors: both the 'static' supervisor with their strategies, and the 'factory' supervisor.

This provides you with a technique to assess your supervision trees.

**Key Takeaways:**

- One tool to understand your supervision trees is by observing the supervision: kill your actors.

**Target Audience:**

- Gleamlins that want to know more about OTP.
- Anyone who wonders about supervision trees.
