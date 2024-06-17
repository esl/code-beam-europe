---
tags:
  - interop
  - rebar3
  - packaging
level: Introductory and overview
title: "Using Elixir in Erlang Projects"
speakers: -_participants/benedikt-reinartz.md

---
Using the newly released exerl set of plugins (https://github.com/filmor/exerl), it's possible to use Elixir seamlessly from previously pure Erlang codebases using rebar3.

Support is implemented and will be demonstrated for
- Adding Elixir itself as a dependency without the need to install it
- Individual Elixir files in src/
- Dependencies that use mix (even "complicated" ones, like packages that use rustler or rustler_precompiled)

**Key Takeaways:**
- Possibility of gradually introducing Elixir into established Erlang codebases
- It's now possible to "tap into" the Elixir ecosystem from Erlang without hassle

**Target Audience:**
- Developers and maintainers of rebar3-built Erlang codebases

