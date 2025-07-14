---
tags: 
  - nif
  - interoperability
  - performance

level: Intermediate
title: "Beyond Your First NIF"
speakers: 
  - _participants/riccardo-binetti.md

---
You've written your first NIF that adds two numbers together, hooray! Now where do you go from here?

This talk digs deeper into the erl_nif interface, showcasing what it offers you for building high performance NIFs.

We will start by learning how to avoid the Cardinal Sin of NIFs, blocking the scheduler. Then we'll move on to handling data more complex than a simple integer. We'll see how to efficiently work with Elixir maps and binaries, and how to safely manage stateful resources that need to be cleaned up by the BEAM's garbage collector.

Did you know that you can monitor a process from a NIF? Or that you can send a message to a GenServer using its registered name? We will go over all the different ways a NIF can interact with the BEAM, extending its capabilities well beyond executing a simple chunk of synchronous code.

NIFs are also capable of bringing the whole BEAM down, so we'll learn some techniques to debug that pesky segfault when things go wrong.

Finally, all the concepts we discuss will be valid regardless of your implementation language. We'll explore the available choices and the libraries that make using each language more ergonomic.

**Key Takeaways:**

- By the end of this session, you will:
- Know how to write NIFs that don't block the BEAM schedulers
- Understand the different ways a NIF can interact and exchange data with the BEAM
- Have a practical approach for debugging NIFs that crash the virtual machine
- Discover the different languages you can use to implement your NIFs and the tooling available for each of them

**Target Audience:**

- Elixir and Erlang developers who have a basic understanding of NIFs and want to learn how to use them effectively in production
- Senior developers looking for optimizing performance-critical parts of a BEAM application
