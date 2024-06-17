---
tags:
  - process-mapping
  - compute-continuum
level: Intermediate
title: "Smart Mapping: Optimizing Compute Across Cloud and Edge in IoT Networks"
speakers: -_participants/peer-stritzinger.md

---
Mapping computational tasks across diverse IoT networks has traditionally been manual, leading to architectural lock-in. This talk explores an innovative approach to developing distributed applications that integrate cloud infrastructure, edge devices, and IoT nodes. We'll discuss mapping compute tasks as Erlang Processes within a dataflow graph onto a heterogeneous network of nodes, guided by criteria such as:
- Statically fixed node mappings
- First-bit latency
- Network and compute bandwidth
- Latency influenced by bandwidth limits
- Energy consumption
- Specialized compute needs
- Data sensitivity and trust
We'll demonstrate this through live demos with cloud and IoT nodes, highlighting how these mappings make use of a compute continuum, meeting all constraints and adapting to changes. 

Join us to explore the intricacies of compute mapping in heterogeneous IoT networks and learn techniques for developing advanced distributed applications leveraging both cloud and edge resources.

**Key Takeaways:**
- Attendees will gain a deep understanding of how to efficiently map computational tasks across heterogeneous IoT networks, leveraging key criteria such as latency, bandwidth, energy consumption, and data sensitivity. The talk will showcase practical implementation strategies, demonstrating the seamless integration of cloud and edge resources to create adaptive, resilient, and secure distributed applications. Real-world demos will illustrate the benefits of this approach, highlighting the optimization of compute power in diverse network environments.

**Target Audience:**
- This talk is tailored for developers, engineers, and architects involved in IoT, edge computing, and distributed systems. While the algorithms are generally applicable and the system also will support containers with arbitrary implementation (on nodes capable of running containers) it will be particularly valuable for developers using languages on the Erlang VM BEAM which opens up much more fine grained mapping and allows us to push processes further towards the IoT/Fog devices with the help of the GRiSP embedded software stack.
- There will be content for all levels of audience from Beginner to Advanced.

