---
tags:
  - LLM
  - testing
  - hallucinations

level: Introductory and overview
title: "Detecting Confident Nonsense: Testing LLM-Driven Apps"
speakers:
  - _participants/hernan-rivas-acosta.md

---
It’s happening to more of us every day: out of nowhere, we’re told to integrate an LLM into the product. And so we do, we wire up a RAG pipeline, we add agents to detect adversarial prompts and we tweak all our system prompts.

And it works! The answers are both fluent and polite, and it even says “I don’t know” when it should. Everything looks great… until a tester reports that the AI promised them a 90% discount or gave dangerously bad advice.

How do we stop that from reaching production, when unit tests can’t validate human language?

In this talk, we'll walk through practical ways to evaluate LLM-driven apps. From the most basic BLEU and ROUGE metrics to aspect-based evaluation, and retrieval scoring; you’ll learn what to measure, when to trust it, and how to catch confident nonsense before your users do.

**Key Takeaways:**

- LLMs need to be tested in a fundamentally different way. We'll look into those ways and why we pick different evaluations for different parts of the problem.

**Target Audience:**

- People suddenly being asked to integrate LLMs into their customer-facing applications.
