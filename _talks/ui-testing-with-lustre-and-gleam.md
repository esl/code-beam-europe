---
tags: 
  - pain-free-ui-tests

level: Introductory and overview
title: "Browsers Need Not Apply, UI Testing With Lustre and Gleam"
speakers: 
  - _participants/hayleigh-thompson.md

---
UI testing is a chore. Often we end up settling with an end-to-end testing system, writing JavaScript assertion and snapshot tests, and dealing with half hour CI times. Isn't there a better way?

In this talk we'll break down and better understand what exactly it is we're trying to test when testing user interfaces before taking a look at four different approaches we can take for UI testing in Lustre without leaving the comfort of eunit.

We'll walk away with a toolkit of testing approaches we can reach for *before* we need to pull out Cypress and grind our CI to a halt!

**Key Takeaways:**

- We'll leave the talk with a toolkit of testing approaches we can reach for without spinning up slow end-to-end tests. And we'll also come away with a greater appreciation that pure functions, static types, and a declarative UI framework means we can place much greater trust in our UIs without needing to *see* them.

**Target Audience:**

- Frontend and fullstack devs that are tired of waiting 30 minutes for CI to fail because a snapshot wasn't updated.

- Backend devs that already don't want to be writing frontend code, let alone testing it.
