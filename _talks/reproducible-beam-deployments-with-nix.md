---
tags: 
  - deployment
  - docker
  - nix
level: Intermediate
title: "Reproducible BEAM Deployments with nix"
speakers: -_participants/norbert-melzer.md

---
Mix or rebar alone do not necessarily produce reproducable artifacts. As they do depend on the system where they run on. Docker at least mitigates the problem with the system libraries, though is it reproducible? No, this is where "nix" comes into place, which allows us to have really reproducible builds. Which can be deployed in various ways.

**Key Takeaways:**
- Mix and rebar do their job well for many things, though not for reproducable builds. And Docker can make them at least "replayable".
- There are so many more tools out in the wild, that do a better job on really reproducable builds. of which one is "nix".

**Target Audience:**
- Open minded "Ops" and "DevOps" persons, as well as developers who wish for a more "pord like development environment"

