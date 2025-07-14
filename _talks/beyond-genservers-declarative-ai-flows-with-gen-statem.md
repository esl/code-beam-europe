---
tags: 
  - aiagents
  - statemachines
  - genstatem

level: Introductory and overview
title: "Beyond GenServers: Declarative AI Flows With gen_statem"
speakers: 
  - _participants/coby-benveniste.md

---
gen_statem is a rarely talked about and used OTP behaviour. Most BEAM developers reach for GenServer when building processes, but in the world of AI agents, gen_statem is the hidden gem that transforms complex agent loops into declarative state machines. Learn why gen_statem's behaviour aligns with AI agent patterns, enabling developers to easily write cleaner code describing how their agents behave. You'll learn how to build gen_statem processes, using features such as state functions, internal events, and postponing to build ReAct (Reasoning/Actions) AI agent loops. This talk is perfect for anyone building AI agents with Elixir wanting to level up their implementation with OTP behaviours.

**Key Takeaways:**

- The main takeaway is that while it is one of the BEAM's "hidden" gems, building AI agents with gen_statem can be a huge advantage over the more classical approach of building with GenServers. When state can have several transitions it is often a great idea to separate it from the data, as opposed to GenServers, where they tend to be combined. The audience will learn how to create gen_statem processes, how the ReAct (Reasoning/Actions) AI agent loop works, and how to build a ReAct loop using gen_statem, using gen_statem features such as state functions, events, and postponing.

**Target Audience:**

- Anyone building AI Agents with Elixir. The target audience should ideally have Elixir experience, and understand basic concepts around processes and pattern matching. No prior experience in gen_statem is needed, we'll build on basic fundamentals during the talk.
