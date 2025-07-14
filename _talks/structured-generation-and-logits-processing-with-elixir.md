---
tags: 
  - structured-deterministic-generation

level: Advanced
title: "Structured Generation and Logits Processing With Elixir"
speakers: 
  - _participants/chris-beck.md

---
When we call an LLM from an application, the result can be a gamble: will it follow the schema, include every required field, or even produce valid JSON? Today we usually validate after generation. If it fails, trigger another generation round that may still break.

There is an alternative: By reaching into the raw, unnormalised token scores (logits) during decoding, we can prune every token that violates a grammar we supply. The model literally cannot create invalid output; no retries, no patch-ups.

This logits-level gating was first published in 2016, yet it remains largely unknown outside a handful of research papers. I’ll surface the idea, show why it slipped under industry radar, and—most importantly—demonstrate how easily you can apply it today with Elixir’s Bumblebee, Nx, and the BEAM’s supervision strengths.

We will see how the technique makes small but critical tasks reliable —emitting strict JSON configs, creating test data, or generating Erlang term syntax—where unconstrained decoding would crumble. 

You’ll leave knowing how to wire grammar constraints into Bumblebee, eliminate brittle post-processing, and ship more reliable, safer Elixir systems.

**Key Takeaways:**

- Built-in guardrails: By filtering tokens at decode time, the model simply can’t stray from your grammar or schema.

- Good-bye, retry loop: No more validate-and-regenerate cycles—latency drops and errors disappear.

- Hidden gem: The approach has been around since 2016, but few teams have discovered it (until now!).

- Easy on the BEAM: Bumblebee and Nx give Elixir developers everything needed to plug grammar constraints straight into their pipelines.

- Real-world wins: Perfect for tasks where the output can be described by a grammar or schema.

**Target Audience:**

- Elixir & BEAM developers who already build services and want tighter control over LLM output.

- Backend engineers concerned about reliability or security.

- Machine-learning practitioners exploring practical inference tricks beyond basic temperature / top-k sampling.

- Tech leads / architects evaluating where structured generation can reduce post-processing and failure handling.
