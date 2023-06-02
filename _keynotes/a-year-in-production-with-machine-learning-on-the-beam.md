---
audience: Everyone.
tags:
	- Machine learning
	- Adoption
	- Data
title: 'A Year in Production with Machine Learning on the BEAM'
speakers:
- _participants/christopher-grainger.md

---
Last year we made the decision to switch our machine learning research, inference, and ETL pipelines to Elixir. Python was our first choice but, with the rest of our codebase in Elixir, we ran into problems with siloing and context shifting. The advent of the Numerical Elixir (Nx) project made the transition possible. The move to an all-Elixir codebase led to streamlining development, less complexity, and swift experimentation -- all force multipliers for a small startup. We've since woven the Nx ecosystem into our workflows, relying on Livebook for daily operations, and rolled out Scholar for a key feature. In this talk, I’ll share our insights and discoveries over the past year since our complete transition to Elixir, how we integrated the Nx ecosystem into our operations, and the practicalities and challenges of managing machine learning in production using the BEAM.

**Key Takeaways for the Audience:**
The Nx ecosystem is ready for production today. It's surprising because of how new it is but, for many, many use cases, it's possible to put machine learning into production only using Elixir. And we're not just talking about trivial things: we run a bespoke large language model (LLM) (that we were able to fine tune in Elixir!) with millions of parameters and run inference with millions of documents each week.

But it's new and there's not a lot of information out there about the practicalities with deployment, or real-world assessments of benefits and challenges. So I can talk to that as a CTO and founder who made the choice and reaped the benefits.