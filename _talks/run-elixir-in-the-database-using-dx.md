---
tags: 
  - ecto
  - simplicity
  - architecture

level: Intermediate
title: "Run Elixir in the database using Dx"
speakers: -_participants/arno-dirlam.md

---
Imagine you could write Elixir code as if all Ecto data is already loaded. With pattern matching to match associations; Enum functions to navigate associated data; accessing fields in associations without a second thought. Even using data from non-associated schemas without having to think about data loading at all, just using Enum functions to slice and dice the data as needed.

This is what the Dx library does. Just like Nx (numerical Elixir) translates Elixir code to run optimized for the GPU, Dx (data-driven Elixir) translates Elixir code to run optimized for the database. It translates your code either to Ecto queries, or to a version with automatic data loading, optimized using batching and concurrency.

This makes for clear and easy-to-read Elixir code that's structured in modules and functions as usual, without any need to implement data loading. The code is easier to maintain and refactor, compared to implementations with Ecto queries and/or preloading, yet efficient.

**Key Takeaways:**
- Getting to know Dx as a new option for data-driven applications
- Lots of examples with code plus what queries it executes
- Application architecture fit: Functional core & Imperative shell
- Restrictions and caveats
- Glimpse into how it's implemented
- State of development and future plans

**Target Audience:**

People:
- working with Ecto a lot
- interested in software architecture
- interested in the Elixir compiler
- interested in new approaches and the overall ecosystem

