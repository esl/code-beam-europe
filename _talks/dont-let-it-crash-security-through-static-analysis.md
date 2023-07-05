---
tags:	
- security, vulnerability detection, static analysis methods
level: Intermediate
title: 	"Don’t let it crash - Security through Static Analysis"
speakers:
- _participants/melinda-tóth.md
- _participants/dániel-horpácsi.md

---
Something to love about the BEAM is the principle of ‘let it crash’: exceptions are isolated and handled by design. Indeed, various kinds of data checks can be mercifully omitted, but it would be rash to conclude that all input validation is redundant and unnecessary. In 2020, the Erlang Ecosystem Foundation curated an extensive list of secure coding principles to raise programmers’ awareness and assist them in creating secure Erlang systems. But the reality is always messy: Erlang/Elixir projects rarely follow these guidelines, and legacy have been running for years with well-known vulnerabilities. In this talk, we will explain how static analysis can be useful for detecting critical security issues in new or legacy Erlang code bases, mitigating and even eliminating them semi-automatically. In particular, we will present use cases of vulnerabilities found in open-source projects and demonstrate how techniques like data-flow analysis can reveal and cure them.

**Key Takeaways:**
- We would like to draw your attention to the fact that security problems exist in Erlang codes. Their detection can sometimes be done with simple tools, but in many cases it is not trivial, and they are difficult to identify. Static analysis methods can help with this. We show problems, solution methods and a tool that can help you detect security vulnerabilities in your code.

**Target Audience:**
- We would like to draw your attention to the fact that security problems exist in Erlang codes. Their detection can sometimes be done with simple tools, but in many cases it is not trivial, and they are difficult to identify. Static analysis methods can help with this. We show problems, solution methods and a tool that can help you detect security vulnerabilities in your code.