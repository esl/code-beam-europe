---
tags:
  - native records datatypes

level: Intermediate
title: "Native Records"
speakers:
- _participants/bjorn-gustavsson.md
published: true

---
Traditional Erlang records are a compile-time convenience; at runtime they are just tuples.

Erlang/OTP 29 introduces native records, a new data type distinct from tuples and maps. In this talk, we'll walk through the motivation behind native records, the design constraints, and practical trade-offs. We'll look at the performance characteristics of the current implementation and how we plan to improve it in OTP 30 and beyond.
