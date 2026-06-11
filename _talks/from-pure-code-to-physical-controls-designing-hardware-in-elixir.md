---
tags:
  - hardware design and modeling

level: Intermediate
title: "From Pure Code to Physical Controls: Designing Hardware in Elixir"
speakers:
- _participants/lucas-sifoni.md
published: true

---
We'll walk through the creation of the hardware control panel of a commissioned installation, from rough sketches and a blank app to the finished product, using Elixir and LiveView. We'll follow a layering philosophy: starting with pure state and transitions, adding behaviour with actors, and composing those small modules into the overall system. LiveView will help us bring those actors together in a visual simulation, which we'll then make alive in hardware, without a code change. In the end, we'll have built a clean separation between logic and IO sources (virtual or physical) by extracting a common behaviour for component types and a normalized event-handling pattern.

The code is released alongside the talk for a deeper dive. While Nerves is used to package the project, it is not the focus of this talk.

**Key Takeaways:**

- You'll walk away with a method to translate software design skills to approach an hardware project, by moving most of the complexity into the software layer, and adapting patterns you already like to use in liveview and functional programming.

**Target Audience:**

- Software developers curious about translating their design skills to the physical world.
