---
tags:
  - Erlang  Tool  Demonstration
level: Intermediate
title: "Mailboxer: Early Detection of Erlang Communication Errors"
speakers: 
- _participants/phil-trinder.md
- _participants/duncan-paul-attard.md

---
The talk presents and demonstrates a new communication checking tool for Erlang codebases: Mailboxer.

If a developer annotates parts of an Erlang codebase with expected message types Mailboxer can statically detect many communication errors in the annotated processes. So errors like unreceived messages, some deadlocks, protocol violations, typos in message tags etc. Finding errors early in development reduces debugging and development times.

Existing session type checkers for Erlang and Elixir enforce channel, rather than mailbox, based communication. In contrast Mailbox types check communication using idiomatic mailbox communication.  Currently Mailboxer targets Erlang, but the type theory and checking technology apply to other actor languages with mailboxes, so Elixir, Scala/Akka and others. 

Erlang will be the first production language to benefit from a radically new communication checking tool.

**Key Takeaways:**
- Adding mailbox types to Erlang code and using the Mailboxer tool can detect communication errors early.
- Mailbox type checkers could soon be available for other BEAM languages soon.

**Target Audience:**
- Developers looking for new tools to apply to their code.
- Tool developers looking explore new tools. 

