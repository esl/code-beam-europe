---
tags:
  - uncommon-beam-optimization

level: Intermediate
title: "Perf & Peep: Lessons From Optimizing a Telemetry.Metrics Reporter"
speakers:
  - _participants/richard-kallos.md
published: false
---
Peep was born in 2023 from the need for a faster Telemetry.Metrics reporter. Since then, with the help of profiling tools like perf-tools and lcnt, it has become even faster.

This talk will go over some bottlenecks that were found in Peep, as well as contributed optimizations that improved performance. The optimizations range from the mundane to the esoteric, offering uncommon insight on how to squeeze the most performance out of the BEAM.

**Key Takeaways:**

- Learn about Peep, a fast Telemetry.Metrics reporter suited to server software that emits large numbers of telemetry events.
- Learn various methods to profile code that runs on the BEAM.
- Learn about common and obscure optimizations for code that runs on the BEAM.

**Target Audience:**

- Developers who build and operate software that emits large amounts of telemetry events.
