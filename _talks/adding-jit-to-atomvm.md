---
tags:
  - atomvm
  - jit
  - llm

level: Advanced
title: "Adding JIT to AtomVM"
speakers:
  - _participants/paul-guyot.md

---
The just-in-time compiler was introduced at CodeBEAM V in 2020 by Lukas Larsson. It shipped with OTP-24 and succeeded HiPE in dramatically improving the speed of the BEAM.

In this talk we will discuss how native code compilation is brought to AtomVM, the virtual machine that runs on micro-controllers and in the browser, following a slightly different approach.

The talk will compare BEAM and AtomVM approaches to emulation. Typically, BeamASM, the JIT compiler of the BEAM, was designed with simplicity and maintenance in mind to cope with the size of OTP team. As AtomVM team is even smaller, simplicity and maintenance are also key requirements. AtomVM's native compiler also needs to address AtomVM's constraints such as portability to most important supported architectures (RISCV, ARM32, Xtensa, WASM) as well as compilation directly on the devices with very few amounts of RAM, as AtomVM can blink with 128 KB of RAM and run Distributed Erlang with as few as 400 KB.

Eventually, AtomVM JIT compiler, being a 2025 project, leverages newest software engineering technologies and the talk will also cover how an LLM eventually helped with such a complex task.

**Key Takeaways:**

- How execution of code in BEAM languages work
- How to software engineer a VM for microcontrollers
- How LLM can be used to compensate for developer knowledge

**Target Audience:**

- Erlang, Elixir and Gleam developers curious about execution of their code
- IoT enthusiasts
