---
tags: 
  - lowpower-edgecomputing-energyharvesting

level: Intermediate
title: "Beyond the Squeeze: Shipping a Full BEAM Stack in 16 MB-Now With Energy-Aware Booting"
speakers: 
  - _participants/peer-stritzinger.md

---
Can a complete Erlang/OTP system truly thrive within just 16 MB of RAM, network effectively, and reliably boot using harvested energy?

At Code BEAM Lite Stockholm, we shared our work-in-progress on fitting the BEAM into an ultra-constrained environment, leaving memory management and energy harvesting as open challenges. Now, we have successfully completed this journey. Memory tuning is optimized enough to comfortably accommodate user applications. We have developed a robust, energy-aware boot sequence that safely initializes Erlang once sufficient harvested energy accumulates. Additionally, we've integrated GRiSP nano fully into GRiSP.io, providing a seamless, reproducible setup for the community.

This talk will highlight allocator diagnostics, memory usage insights, and live demonstrations of efficient low-power operation. Attendees will gain practical knowledge on extreme optimization, insights into designing energy-conscious boot processes, and an understanding of how to reliably deploy BEAM-based solutions in environments previously considered unreachable.

**Key Takeaways:**

- Memory Optimization Techniques: General strategies for significantly reducing memory footprints, including allocator tuning, module management, and runtime adjustments.

- Energy-Aware System Design: Insights into constructing boot sequences and runtime behaviors that adapt dynamically to available harvested energy.

- Integration and Deployment Best Practices: Learnings from integrating highly optimized Erlang runtimes with minimal OS environments such as RTEMS.

- Community Tooling Insights: How accessible, reproducible tooling, such as GRiSP.io, simplifies the deployment of constrained embedded Erlang applications for the broader community.

**Target Audience:**

- Embedded and IoT System Developers interested in using Erlang/Elixir and the BEAM in resource-constrained hardware environments, such as GRiSP and GRiSP nano platforms.
- BEAM Enthusiasts and Erlang/Elixir Developers keen on advanced optimization techniques and exploring the limits of Erlang/Elixir runtimes in non-traditional deployments.
- Low-Power and Energy-Harvesting Experts looking for insights into integrating energy-aware boot and runtime management for sustainable computing.
- Real-Time System Engineers seeking practical lessons from deploying Erlang/Elixir with RTEMS or similar real-time operating systems.
- Researchers and Innovators exploring novel applications of functional programming and fault-tolerant technologies in ultra-low-power scenarios.
