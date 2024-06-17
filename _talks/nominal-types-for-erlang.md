---
tags: 
  - Erlang
  - Types
  - Dialyzer
level: Introductory and overview
title: "Nominal Types for Erlang"
speakers: -_participants/isabell-huang.md

---
Nominal typing has been used in many dynamically typed languages. User-defined types are distinguished by their names. As my master thesis at Uppsala University, I propose the addition of nominal types '-nominal' in Erlang, where the changes can be applied exclusively to Dialyzer (modulo parsing). As a side effect, nominal types can encode opaque types, which improves Dialyzer's maintainability. Nominal types will be an upcoming feature for OTP 28.

**Key Takeaways:**
- Understanding how nominal types can be defined and used in Erlang. 
- Understanding how Dialyzer performs type-checking for nominal types, and the advantages of encoding opaques internally as nominal types.

**Target Audience:**
- Erlang developers and enthusiasts for type systems

