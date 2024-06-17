---
tags:	
- type-checker, etylizer, static analysis
level: Intermediate
title: 	"etylizer: Set-theoretic Types for Erlang"
speakers:

---
Erlang’s type language provides powerful such as parametric polymorphism, equi-recursive types, as well as singleton, union, and (a variant of) intersection types.
But its type signatures mainly serve as documentation as language features such as pattern matching and dynamic type tests complicate the design of a static type system.

In our talk, we present etylizer, a static type checker for Erlang that adopts set-theoretic types as its foundation. With a demo on selected case studies, we will demonstrate how existing Erlang code can be statically typechecked without or with only minor modifications to the code. We will further show how set-theoretic types can enhance the development process and improve code quality for idiomatic Erlang code. The etylizer project is funded by the Erlang Ecosystem Foundation and developed as free open-source software <a href=https://github.com/etylizer>here</a>.

**Key Takeaways:**
- How to read and interpret type annotations in Erlang.
- Ideas behind set-theoretic types and how they are applicable to Erlang.
- Benefits of static typing with etylizer, e.g., exhaustiveness checks for pattern matching.
- How to engage in the etylizer project.

**Target Audience:**
- Erlang developers that are curious how Erlang would benefit from static typing.