---
tags:
  - CyanView + Elixir = Broadcast. Reliability. Scale.

level: Introductory and overview
title: "From Super Bowl to Olympics: How CyanView Powers the World's Biggest Broadcasts With Elixir"
speakers:
  - _participants/daniil-popov.md
  - _participants/david-bourgeois.md

---
Discover how a 9-person Belgian startup revolutionized live broadcast technology using Elixir. CyanView controls 200+ cameras simultaneously during major events like the Olympics, Super Bowl, NBA, and NFL broadcasts—all without a marketing budget, growing purely on technical excellence.
This talk reveals how Elixir's fault-tolerant architecture solved critical challenges in broadcast camera control. Learn about their MQTT + GenServer design that handles millions of real-time events, LiveView running on embedded ARM hardware, and supervision trees that prevent single camera failures from cascading across entire broadcasts.
We'll explore real-world examples including their Olympics Beijing deployment—controlling 100+ cameras from Paris with zero broadcast failures despite intercontinental latency. See how binary pattern matching enables rapid protocol reverse engineering, allowing quick integration of new camera types and features like gimbal control.

**Key Takeaways:**

- Explain CyanView use-case more detailed and present how Elixir can be used in broadcasting domain.

**Target Audience:**

- Perfect for developers interested in IoT, real-time systems, and mission-critical applications where "you only get one chance." Witness how the right technology choice enabled a tiny team to transform an entire industry.
