---
tags: 
  - performance
  - static-analysis
  - Dialyzer
level: Intermediate
title: "Scaling Dialyzer"
speakers: -_participants/tom-davies.md

---
Dialyzer is a powerful tool for finding bugs in Erlang code, and as a codebase grows, it becomes harder for humans to keep track of everything themselves, so we need to increasingly lean on our tooling to get the job done.

In OTP 26, Dialyzer's incremental mode became widely available, allowing Dialyzer's performance to scale to larger codebases by avoiding redundant analysis between code changes.

In this talk, I will cover the next steps in scaling Dialyzer's performance which I have been working on: including finer-grained incrementality, micro-optimisations, ETS performance, and more.

Whilst the talk is primarily about Dialyzer, the performance considerations and optimisations may be of wider interest to other people working on the BEAM.
