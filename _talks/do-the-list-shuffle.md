---
tags:
  - Algorithms
  - Data structures
  - Optimization

level: Intermediate
title: "Do the List Shuffle"
speakers:
- _participants/raimo-niskanen.md
published: true

---
A description of the selection and development of the new list shuffle algorithm in the `rand` module in OTP 29, what makes the different possible algorithms fast or slow, and how to optimize them.

We look at known shuffling algorithms, where *functional* ones are hard to find online, study their implementation in Erlang, benchmark how they perform with the garbage collector, show some optimizations, and arrive at the chosen algorithm that the author could not find on the Internet.

**Key Takeaways:**

- How some data structures and algorithms perform in the BEAM, and ways to optimize them, by looking at what seems to be the fairly simple problem randomly shuffling of a list of elements.

**Target Audience:**

- Developers interested in the performance of common Erlang/Elixir data structures and algorithms.
