---
tags:
  - elixir-rust-interop

level: Intermediate
title: "The BEAM-Rust Sandwich"
speakers:
  - _participants/julian-koepke.md

---
The BEAM is the perfect tool for building distributed systems that are resilient, maintainable and fun to implement. However, there are certain areas where the BEAM lacks, like computation heavy and graphically intensive applications.

In this talk I will demonstrate why Rust is the perfect match for Elixir. You will learn how to build a Phoenix LiveView application that is sandwiched between Rust, in the browser using WebAssembly, and in the backend using Rustler. Whether you're planning to build a browser game with 3d graphics, a weather simulation or just want to calculate the last digit of Pi, there is no excuse not to run the BEAM anymore.

**Key Takeaways:**

- This is a guided tour through the architecture of a Phoenix LiveView application that leverages Rust where Elixir falls short.

- Targeting the browser, we will inspect how to compile a Rust module to WebAssembly, serve it through Phoenix and embed it in LiveView. Then we will look into how to call the same Rust code as a NIF using Rustler in the backend. To round it up, there will be a demo running both together in one web application.

**Target Audience:**

- Everyone who wants to learn how to overcome the limitations of the BEAM using Rust. No prior knowledge of Rust is required to follow this talk, but you should bring some interest in learning it. We will not go into specifics of the Rust language, but I will guide you through all the nitty-gritty details of setting up your LiveView application to interface with Rust.
