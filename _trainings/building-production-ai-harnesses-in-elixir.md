---
experience:
- Intermediate
title: "Building Production AI Harnesses in Elixir"
type: tutorial
event_date: 20 Oct 2026
venue: TBC
trainers:
- _participants/chris-beck.md
---
Over a full day, you'll go from an empty Mix project to a working, reliable agent harness, writing the code at each step. We'll start exactly where the talk does: a naive agent on a deliberately weak model, failing at a simple task and lying about it. By the end of the day, you'll have wrapped that same untrustworthy model in a harness solid enough to trust with a real job — without ever touching the prompt.

What we'll build, module by module:

* **The bare agent loop.** A GenServer-driven loop that calls a model, executes tools, and accumulates a trace. We'll watch it fail honestly so we understand what we're actually fixing.
* **A tool registry.** Defining, registering, and dispatching tools the agent can call, with clean boundaries between what the model decides and what your code executes.
* **Guardrails the OTP way.** Capping iterations, compressing context, and enforcing limits — then making them robust by letting supervision handle the failure modes instead of defensive code.
* **A deterministic verification step.** Inspecting the trace to catch hallucinated successes, so a failed run reports failure instead of lying.
* **Programmatic handlers.** Pulling sensitive or must-be-correct steps (auth, side effects, anything you can't trust to a model) out of the agent's hands and into deterministic, supervised code.
* **Putting it under a supervisor.** Turning the whole thing into a proper OTP application where a crashing or misbehaving agent run is a recoverable event, not an outage.

**Format:** Short framing segments followed by guided, hands-on exercises. You'll write real Elixir at every stage. We'll work against a shared starter repo, and each module builds on the last, so you leave with a complete harness you understand end to end — not a black box you copied.

**Duration:**
* 8 hours

**Tutorial objectives:**
By the end of this workshop, participants will be able to:

* Define an agent harness from first principles and identify its core components — tool registry, context management, guardrails, agent loop, and verification step — in any agent system they encounter.
* Build an agent loop in Elixir that calls a model, dispatches tools, and accumulates an inspectable trace, structured as a GenServer.
* Design and register tools with clean boundaries between what the model decides and what application code deterministically executes.
* Implement guardrails that cap iterations and compress context, and recognize when to enforce limits in code versus when to let supervision handle a failure.
* Write a deterministic verification step that inspects an agent's trace to catch hallucinated or falsely-reported successes.
* Extract untrusted steps into programmatic handlers, moving authentication, side effects, and must-be-correct logic out of the model's control and into supervised, deterministic code.
* Structure a harness as a proper OTP application, so that a crashing or misbehaving agent run becomes a recoverable event rather than an outage.
* Map OTP primitives to harness design, articulating why supervision trees, process isolation, and "let it crash" are a strong fit for reliable agent infrastructure.
* Evaluate reliability as the primary lever for production agents, and apply harness patterns to reduce cost and improve trustworthiness using cheaper or smaller models.

**Target audience:**
This workshop is for intermediate to advanced Elixir and Erlang developers who want to build reliable AI agents, not just hear about them. The day is spent writing code, so you should be comfortable working in a Mix project and reading OTP code (GenServer, supervisors) without hand-holding. No machine learning background is required — the entire focus is the engineering layer around the model, and we treat the model itself as a black box.

It will be most valuable for:

* Backend and platform engineers who are bringing LLMs into production systems and need them to behave reliably under real conditions, not just in a demo.
* Teams already running agents — in Elixir or any other language — who are hitting reliability walls like hallucinated successes, runaway token costs, and brittle prompt-tuning, and want a durable architectural answer.
* Elixir developers exploring where the BEAM fits in the AI stack, who suspect OTP has something concrete to offer here and want to build it with their own hands.
* Tech leads and architects evaluating whether to standardize agent infrastructure on Elixir, who want enough hands-on grounding to make that call.

This workshop is not a fit for complete Elixir beginners (the pace assumes working fluency) or for ML researchers seeking model-training or fine-tuning content — we don't touch the inside of the model at all.

**Prerequisites:**

*Skills*
* Working fluency in Elixir: comfortable in a Mix project, writing modules and functions without a reference open.
* Ability to read and reason about basic OTP code — GenServer and supervisors in particular. You don't need to be an expert, but the harness is built on these, so they shouldn't be unfamiliar.
* General command-line comfort (running mix tasks, managing environment variables).
* Only brief machine learning or AI background required. We treat the model as a black box and focus entirely on the engineering around it.

*Software & setup*
* A laptop with a recent Elixir and Erlang/OTP install (specific versions confirmed in a setup email before the session).
* The starter repo cloned and dependencies fetched (mix deps.get) before arriving — a setup email with exact steps goes out ahead of time so we can start building, not installing.
