---
tags:
  - FLAME
  - Oban
  - ETL
level: Intermediate
title: "Using FLAME and Oban for ETL"
speakers: -_participants/christopher-grainger.md

---
FLAME (Fleeting Lambda Application for Modular Execution) is a new approach to Lambda architectures, copying your entire app for fast and easy execution on short-lived architecture.

At Amplified, we've migrated our ETL (extract, transform, load) from multiple apps across multiple clouds using RabbitMQ as an event bus to go all in on a monolithic architecture using FLAME and Oban.

Consolidating into a monolith using this combination has permitted us to dramatically simplify our codebase, making it easier to leverage the built-in conveniences of Phoenix and LiveView like Phoenix.PubSub. This gave us the freedom and confidence to build ETL-driven features that integrate tightly with our SaaS app, including real-time updates for our users.

This talk will focus on the transition from building infrastructure for the BEAM towards building infrastructure with the BEAM. FLAME offers a new paradigm for ‘BEAMOps’, and this talk will highlight emergent patterns and benefits.

**Key Takeaways:**
- How FLAME and Oban can be leveraged to simplify infrastructure as code, integrate infrastructure provisioning into application code, and more easily build real-time features for end users.

**Target Audience:**
- Anyone who works with infrastructure as code and wishes they could drive more from their application code. Anyone who wants to simplify their stack and consolidate their codebase.

