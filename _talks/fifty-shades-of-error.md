---
tags: 
  - devx
  - productivity
  - testing

level: Introductory and overview
title: "Fifty Shades of Error"
speakers: 
  - _participants/roberto-aloi.md

---
"assert" is a brand new library for Erlang, designed at WhatsApp, which enhances how Erlang errors and assertions are rendered, making it easier for developers to understand what is wrong when an error occurs.

A drop-in replacement for Erlang/OTP stdlib's assert macros and inspired by Elixir's ExUnit library and the Exception behaviour, "assert" includes a structural diffing library and an exception blaming mechanism for Erlang.

In this talk you will learn how the library can help your productivity and how to use it. We will also explore the technical implementation behind "assert".

"assert" is an example of how BEAM languages can influence each other, driving innovation and improvement across the whole ecosystem.

**Key Takeaways:**

- Simple visual enhancements can lead to smarter debugging and more efficient development cycles
- "assert" can be a precious tool in your debugging toolbox
- BEAM languages can heavily inspire each other

**Target Audience:**

- Erlang developers and enthusiasts
- Anyone who will ever write or debug an Erlang test
