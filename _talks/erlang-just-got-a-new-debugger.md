---
tags: 
  - debugger

level: Introductory and overview
title: "Erlang Just Got a New Debugger"
speakers: 
  - _participants/daniel-gorin.md

---
OTP 28 comes with new debugging capabilities and edb is a stepping debugger built around them. Unlike OTP's old debugger, edb will freeze your node and let you check what all those processes are up to, with no rush. 

Is this a toy? Not at all! We use it at WhatsApp everyday and, as we will see in this talk, so can you.

**Key Takeaways:**

- There's a new debugger for Erlang (requires OTP 28)
- Works with VSCode or any major editor/IDE
- Not much is Erlang specific, shouldn't be too hard to support other BEAM languages
- They may want to try it out

**Target Audience:**

- Erlang / Elixir / Gleam developers
