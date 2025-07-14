---
tags: 
  - core-erlang
  - formal-methods
  - proven-correct-software

level: Intermediate
title: "Formally Based Tools for Safer Erlang"
speakers: 
  - _participants/peter-bereczky.md
  - _participants/daniel-horpacsi.md

---
Ensuring program correctness (particularly in concurrent systems) is a complex challenge. Subtle bugs often arise from unexpected interactions or code changes and may go undetected until they cause failures in production. Formal methods help address these challenges by providing mathematically precise definitions and proofs of program behaviour. This talk focuses on Core Erlang, an intermediate language used within the Erlang compiler, and its precise implementation using the Coq/Rocq proof management system.

We explore practical tools built on this foundation, such as verifying program correctness and ensuring that refactorings and optimisations preserve behaviour without relying on testing. We also present a formally based interpreter for Erlang that validates our definitions against the behaviour of Erlang/OTP. Beyond serving as a reference implementation, our interpreter also enables systematic exploration of possible schedulings in concurrent programs, aiding developers in code comprehension. Our formal model also supports a long-term goal: developing a verified Erlang compiler free from miscompilation issues.

**Key Takeaways:**

- Formal methods can be applied to Erlang: They offer a principled approach to ensuring program correctness, particularly in concurrent systems.
- Core Erlang has a formal definition in Coq/Rocq: The intermediate language used by the Erlang/OTP compiler is precisely modelled in the Coq/Rocq proof management system.
- Formally based tools for Erlang are actively developed: These tools support verification of program correctness and help developers better understand and reason about their code.
- Toward a verified Erlang compiler: This work serves as a foundation for the long-term goal of developing a compiler with formally proven correctness, eliminating miscompilation risks.

**Target Audience:**

- For anyone who is interested in applying formal methods and machine-assisted theorem proving to develop trustworthy software
