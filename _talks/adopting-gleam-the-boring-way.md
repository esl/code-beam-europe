---
tags: 
  - gleam-lustre-production

level: Intermediate
title: "Adopting Gleam the Boring Way"
speakers: 
  - _participants/yoshi-reusch.md

---
You've learned about Gleam and are eager to use it in practice - but introducing a new  language raises important questions: How will it integrate with your existing codebase? What if functionality isn't available yet? Where does introducing Gleam even make sense?

Good news: adopting Gleam doesn't have to be an all-or-nothing decision! In this talk, we'll explore practical patterns for incremental adoption: identifying low-risk "islands" for Gleam, calling Gleam from Erlang/Elixir/JavaScript, and integrating existing libraries when you need them.

Through real-life FFI examples covering both backend integration and how to add Lustre to your frontends, you'll leave with a toolkit for bringing Gleam to production without the big rewrite.

**Key Takeaways:**

- How to identify if Gleam would be a good fit and finding the right niches
- How Gleams FFI mechanism lets you call Erlang, Elixir and Javascript functions and how to annotate them
- When to use FFI type assertions vs the dynamic/decode API
- Best practices on writing good Gleam APIs around native libraries
- Different techniques on how to integrate Gleam in existing Elixir, Erlan,g and frontend Javascript apps

**Target Audience:**

- software architects and engineers evaluating tools for production systems.
