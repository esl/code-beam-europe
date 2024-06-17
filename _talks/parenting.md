---
tags:
  - parenting is hard
level: Intermediate
title: "Parenting"
speakers: -_participants/sasa-juric.md

---
This is a tutorial on managing process hierarchies with OTP, with a special focus on "smart parents", i.e. worker processes which start their own children. The talk will present not-so-obvious pitfalls of naive start-linking, and explain proper steps to handle the children. You'll also learn about the library, which, by including a missing layer between GenServer and Supervisor, makes the parenting job much easier. Finally, the talk will present a fully reimplemented and reimagined supervisor behaviour 🙈

**Key Takeaways:**
- learn about parent responsibilities
- see an example of bottom-up layered design
- challenge some established patterns

**Target Audience:**
- Developers who are familiar with OTP behaviours, such as GenServer and Supervisor. The code examples will be in Elixir, but Erlang & Gleam devs should find it interesting too.

