---
tags: 
  - erlang
  - jit
  - arm32

level: Intermediate
title: "BeamAsm Goes Embedded: Porting Erlang’s JIT to ARM32"
speakers: 
  - _participants/peer-stritzinger.md
published: true

---
BEAM JIT (BeamAsm) made Erlang/OTP faster on x86-64 and ARM64, but ARM32 — still common in embedded, industrial and IoT systems — was missing. This talk tells the story of closing that gap.

Peer will walk through the practical journey of bringing the Erlang JIT to ARM32: cross-building OTP, running and debugging under qemu-arm and gdb-multiarch, teaching AsmJit and BeamAsm about ARM32’s smaller register file, tagged terms, literal pools and PC-relative displacement limits, and chasing the kind of bugs where a single NOP can make a crash disappear.

The talk is not a tour of every emitter. It is a guided path through the constraints, failures and design choices that turned “halt(42)” into a working Erlang shell, then into a completed JIT running on a GRiSP2 board. We will end with fresh GRiSP2 benchmarks and what this means for Erlang on embedded ARM devices.

Attendees will leave with a clearer mental model of how BeamAsm works, why VM ports are harder than “just emitting assembly,” and concrete lessons for debugging generated code.

**Key Takeaways:**

- What it takes to bring Erlang’s BeamAsm JIT to a new CPU architecture, using ARM32 as a concrete case study.
- Why ARM32 is more challenging than “just another ARM target”: fewer registers, different calling conventions, literal pools, PC-relative limits, tagged Erlang terms, and tight embedded constraints all influence the design of the JIT.
- Practical techniques for debugging generated machine code, including cross-building OTP, running under QEMU, using gdb-multiarch, and tracking down bugs where tiny instruction-layout changes can alter program behaviour.
- How the engineering work connects to real-world impact: a completed ARM32 JIT running on a GRiSP2 board, with fresh benchmarks showing what BeamAsm can mean for embedded Erlang systems.

**Target Audience:**

- Erlang/Elixir developers who are curious about what happens below the language level: the BEAM VM, BeamAsm, JIT compilation, native code generation, and runtime performance.
- People working with embedded Erlang, IoT, industrial systems, GRiSP boards, or ARM-based devices, especially those interested in getting more performance out of constrained hardware.
- Compiler, VM, and systems programmers who enjoy the low-level parts: register allocation constraints, calling conventions, tagged values, generated assembly, cross-compilation, QEMU, and GDB debugging.
- No prior experience with JIT compiler implementation is required. The talk is intended for a technically curious Code BEAM audience that wants to understand the engineering journey, the trade-offs, and the practical lessons from bringing BeamAsm to ARM32.
