---
tags:
  - Declarative
  - Relational
  - Reactive

level: Introductory and overview
title: "Saying What — A New Declarative Language for the BEAM"
speakers:
- _participants/alejandro-ramallo.md
published: true

---
A first public introduction tour to Bondy is a new BEAM language that Leapsight is developming for the implementation of MAMPaS (MultiAgent MultiParty Systems). 

Bondy is built around one idea: values, types, patterns, relations, rules and processes all live in one uniform algebra of constraints. At the bottom is the Shape — a constraint value in the Typed Feature Structure tradition: types, values and patterns are the same kind of object, inheritance is sort ordering, unification refines everything. On top, Hindley–Milner principal type inference instantiates HM(X) over the Shape algebra; the solver is itself written in Bondy. 

Every layer above reduces to constraints over it: a typed relational model with pluggable adapters (ETS, Postgres); a Rules engine for reactive rules; a Datalog engine for deductive queries with provenance; and GenReactor — a new OTP behaviour for processes whose state is a set of constraints the runtime keeps consistent. 

An early version of Bondy is being used in a production system today by Leapsight clients. The first public release of the languague will be announced during the talk (OSS / Apache 2).

**Key Takeaways:**

- What Bondy is and where it fits: a self-hosted, statically typed, declarative language for the BEAM, organised around one semantic substrate — Typed Feature Structures — with every layer above (types, relations, rules, processes) reducing to constraints over it.
- The unifying idea: a single algebra in which types, values, and patterns are the same kind of object, inheritance is sort ordering rather than method dispatch, and unification is the universal way to refine information.
- The synthesis at the heart of the language: Hindley–Milner principal type inference instantiated over the Shape algebra — semantic richness from the substrate, let-polymorphic principal types from inference — implemented as a Constraint Handling Rules (CHR) program written in Bondy itself, growing into type classes with algebraic laws and first-class effect rows.
- Relations and rules as first-class substrates: typed relations with pluggable adapters (ETS, Postgres); a CHR engine for forward-chaining and reactive rules; a Datalog engine for deductive queries with provenance —  coexisting as separate engines over the same Shape algebra.
- GenReactor as a new OTP behaviour: a process specified as a set of invariants and rules over relations rather than handle_call/handle_cast clauses, kept consistent by the runtime.
- Where Bondy is going: federated multi-agent systems, provenance-tracked data, CRDTs and reactive Fluents/Signals as further constraint families — and an honest view of what works today versus what's on the  roadmap.

**Target Audience:**

- BEAM developers (Erlang, Elixir, Gleam) who are curious about new languages on their VM; anyone interested in static typing for distributed and reactive systems; users of Datalog, Datomic, XTDB, Soufflé, or Differential Dataflow who want a typed BEAM-native equivalent; computational-linguistics and knowledge-representation folks who recognise Typed Feature Structures; and developers drawn to declarative paradigms — feature-structure unification, relational and deductive databases, logic and constraint programming, reactive rules — who want to see them baked into the language rather than bolted on as a library.
