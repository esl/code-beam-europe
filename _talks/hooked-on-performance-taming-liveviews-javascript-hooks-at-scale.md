---
tags:
  - Phoenix LiveView performance

level: Intermediate
title: "Hooked on Performance: Taming LiveView's JavaScript Hooks at Scale"
speakers:
- _participants/matt-swensen.md
published: true

---
Phoenix apps are famously lean on JavaScript…until they aren't. LiveView makes it easy to ship rich and performant UI fast, but as your app matures and hooks accumulate, frontend performance demands real attention. All hooks must be loaded and registered before LiveView boots, so in an aging production codebase, heavy dependencies like React bloat every page load. The BEAM gives you outstanding time-to-first-byte, but those gains get undermined if the browser still has to download, parse, and execute tens of MB of JavaScript before your user can interact with the page.

At Jump, we tackled this in a codebase exceeding 1.5 million lines of Elixir and 150 thousand lines of JavaScript by combining native ES module loading, esbuild bundle splitting, and a custom `LazyHook` that defers loading hooks until they're actually needed. We'll walk through the `LazyHook` implementation in detail—which we've open-sourced for the Phoenix/LiveView community—along with the trade-offs and the measurable wins.

**Key Takeaways:**

- Audience members will come away with a simple and practical solution for improving their page load times on the front end.

**Target Audience:**

- Phoenix developers with large codebases
