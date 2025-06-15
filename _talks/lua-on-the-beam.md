---
tags:
  - Lua in Erlang
level: Intermediate
title: "Lua on the BEAM"
speakers:
- _participants/dave-lucia.md
- _participants/robert-virding.md
published: false

---
Luerl is an implementation of the Lua parser, compiler, and runtime, written in pure Erlang. It allows Lua programs to be executed on the BEAM in a fully sandboxed environment, while allowing integrators to expose Erlang and Elixir functions directly to Lua programs.

In this talk, Robert Virding will give an overview of Lua and the Luerl implementation discussing some of the issues which arise and how they are solved and the added power they can give. We will cover a brief history of Lua, what makes Luerl unique, and how it executes Lua code.

To demonstrate how Luerl can be used in real products, Dave Lucia will showcase how his company, TV Labs, uses Lua to provide a customer-facing scripting interface for testing Smart TV applications. Using TV Labs, Dave will spin up a physical television in his web browser, navigate through a Smart TV app, take screenshots, and perform computer vision tasks, all within the Lua environment.

**Key Takeaways:**
- Understanding how the Erlang/Elixir system can be extended in a useful, powerful and safe way while still preserving the basic features of the BEAM.

**Target Audience:**
- System developers, programming language enthusiasts, and curious web-developers
