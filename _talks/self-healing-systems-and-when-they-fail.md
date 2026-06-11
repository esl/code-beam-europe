---
tags:
  - Self-Healing
  - Architechural Failures
  - OTPMechanisms

level: Intermediate
title: "Self-Healing Systems and When They Fail"
speakers:
- _participants/spoorthy-sridhara.md
published: true

---
Talk is about Designing Supervisor Trees That Actually Recover and also When the Supervisor Can't Save which is failure ways that OTP doesn't catch much. Designing supervisor trees tells Beyond the basics of one_for_one,  talk digs into sophisticated supervision strategies for production systems, covering rest_for_one, dynamic supervisors, circuit breakers built from GenServers, and the difference between a system that restarts and a system that genuinely recovers with preserved state. Having said on the design can also reflect upon what Supervision trees doesnt handle —like ETS table bloat, message queue floods, and cascading timeout storms and couple others. This talk catalogs the production failure modes that OTP's built-in mechanisms don't address, and presents the monitoring, alerting, and architectural patterns that do. Would be demonstrating examples from my own industry experiences where i have personally faced them

**Target Audience:**

- erlang begineer/ intermediate
