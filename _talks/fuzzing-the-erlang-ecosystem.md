---
tags:	
- fuzzing, scoping, tools
level: Intermediate
title: 	"Fuzzing the Erlang Ecosystem"
speakers: _participants/robin-morisset.md

---
Erlfuzz is a recently open-sourced tool that produces random valid Erlang programs, used to test erlc, the BEAM VM, and a variety of other tools (dialyzer, eqWAlizer, erlfmt, infer, etc..). It has found more than 80 bugs to date, including more than 60 bugs in erlc.
In this talk I'll explain how erlfuzz works, what tricks were used to detect subtle VM bugs, and how to use it for any tool you may want to test. I'll also mention some of the dark corners of the language that it revealed, mostly around the Erlang scoping rules.

**Key Takeaways:**
- Fuzzing is a very generic bug-finding technique that can be used to find many kinds of bugs in most tools.
- Various important points to make fuzzing work in practice, e.g. having a good test case minimizer, avoiding trivially invalid inputs, finding good correctness oracles.
- Erlang scoping rules are weird and inconsistent, but they are now documented.

**Target audience:**
- people interested in fuzzing tricks and bug-finding techniques in general
- people who work on any tool ingesting Erlang code
- people who are simply curious about dark corners of the language, such as its scoping rules.