---
tags: 
  - oban
  - resilience
  - pragmatism

level: Intermediate
title: "Taming 20 Million Oban Jobs in Production"
speakers: 
  - _participants/karlo-smid.md

---
What happens when a queue meant for thousands of jobs swells to 20 million—and keeps growing? In this talk, I’ll walk you through a real-world incident where our Oban queue spiraled out of control in production. We’ll dissect what led to this situation, how we investigated the root cause without halting traffic, and the changes we made to restore stability. This isn’t just a story about background jobs—it’s a practical lesson in diagnosing live systems, managing back pressure, and making safe trade-offs in production.
As a bonus, I’ll share battle-tested design tips for building resilient systems with Oban—from queue isolation and job retries to rate-limiting and observability. Whether you’re scaling a system or preventing your own “20 million jobs” moment, these lessons will help.

**Key Takeaways:**

- Strategies for debugging and resolving large-scale queue backlogs

- Practical advice for running Oban in production environments

- How to design job-processing systems that are resilient and observable

- Techniques for managing job volume, retries, and queue isolation

- Bonus tips from real-world experience designing with Oban

**Target Audience:**

- Elixir developers, DevOps, and engineering leads working with or planning to adopt Oban.
