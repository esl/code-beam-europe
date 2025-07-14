---
tags: 
  - concurrent
  - resilient
  - evaluation

level: Introductory and overview
title: "Concurrent AI Evaluation: Scaling Model Performance Monitoring With OTP"
speakers: 
  - _participants/ramiro-matteoda.md

---
Evaluating model performance remains a significant challenge in the rapidly evolving AI landscape. Traditional evaluation approaches often struggle with scale, consistency, and real-time feedback integration—precisely the problems that Elixir and the BEAM were designed to solve.

We'll explore:

Live Benchmarking Pipelines: Implementing resilient GenServers and dynamic supervision trees that continuously process evaluation data at scale.

Concurrent Prompt Evaluation: Building distributed worker pools that can evaluate thousands of prompt variations across multiple LLM providers.

Systematic Human-in-the-Loop Automation: Designing resilient feedback processing pipelines using GenStage and Broadway that validate human annotations, detect inconsistent labelers, and automatically route corrections into training loops.

LangChain.ex Integration: Implementing "LLM-as-a-judge" evaluation patterns using LangChain.ex to create sophisticated, criteria-based evaluations of AI outputs with minimal code overhead.

This talk demonstrates why Elixir's unique strengths make it the ideal platform for building AI evaluation systems that scale from prototype to production.

**Key Takeaways:**

- This talk aims to bridge the gap between theoretical AI evaluation concepts and practical, production-ready implementations using Elixir's unique capabilities. The audience will learn:

- 1. How to design and implement scalable AI evaluation architectures using OTP principles
- 2. Practical patterns for handling the inherent uncertainty in AI evaluation (timeouts, rate limits, inconsistent results)
- 3. How to integrate human feedback loops into automated evaluation pipelines
- 4. Working code examples using LangChain.ex and other Elixir AI libraries that they can adapt for their own projects

**Target Audience:**

- Elixir developers working with AI/ML systems, AI engineers interested in scalable evaluation architectures, and teams building production LLM applications who need robust monitoring solutions.
