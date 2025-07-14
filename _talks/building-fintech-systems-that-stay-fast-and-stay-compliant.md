---
tags: 
  - fintech-compliance-beam

level: Intermediate
title: "Building Fintech Systems That Stay Fast and Stay Compliant"
speakers: 
  - _participants/erik-stenman.md

---
Most fintech backends either grow too fast and break, or slow down to stay compliant. It doesn’t have to be either-or.

This talk is a practical overview of how to design systems that can handle regulation, scale, and product changes at the same time. I’ll share patterns I’ve used across different fintech projects: payment flows, ledgers, orchestration, and audits.

Some of it is low-level: typed money, trace IDs, and structured logs. Some of it is design choices: clear ownership, process boundaries, and how to support change without adding risk.

I’ll also touch on what the BEAM makes easier in this kind of environment, and where you still have to think for yourself. No frameworks, no buzzwords. Just decisions that hold up under pressure.

**Key Takeaways:**

- What a system needs to support compliance without blocking teams
- Practical patterns for ledgers, orchestration, and audit trails
- Trade-offs that show up late if you ignore them early
- Why BEAM is a strong fit for regulated infrastructure

**Target Audience:**

- Developers, tech leads, and architects working on fintech systems or regulated platforms
