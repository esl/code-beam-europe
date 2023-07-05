---
tags:	
- DSL, NimbleParsec, Ecto
level: Intermediate
title: 	"Craft your Domain-Specific Query Language with NimbleParsec and Ecto"
speakers:
- _participants/riccardo-binetti.md

---
Imagine you want to ask your API ""List all devices which are not located in Europe and are currently connected or are either tagged 'maintenance' or 'retired'"". Expressing this kind of  selection with query parameters quickly becomes unwieldy, and even a more structured query language like GraphQL can feel clunky to express this, especially if the target user is not a technical one.

Ideally, we'd want users to be able to write something like:
(not attributes[""continent""] == ""EU"") and (connected or (""maintenance"" in tags or ""retired"" in tags))

In this talk I will show you how this can be achieved with the power of Elixir, NimbleParsec and Ecto.

We will use NimbleParsec to parse the domain-specific language into an Abstract Syntax Tree represented using Elixir structs, and then we will traverse that AST to produce a valid query using the power of Ecto dynamic queries.

**Key Takeaways:**
- "The main takeaway of the talk is showing how NimbleParsec can be used to easily create domain-specific languages for different purposes, in this case combining it with Ecto dynamic queries.

**Target Audience:**
- Anyone with some previous Elixir (and possibly Ecto) experience