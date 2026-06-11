---
tags:
  - Adoption
  - mentorship
  - functional

level: Intermediate
title: "Ruby Crimes in Elixir Codebases"
speakers:
- _participants/travis-fantina.md
published: true

---
Working for an agency that once primarily worked in Ruby I've been able to examine two Elixir monoliths built two years apart (by the same developer). This has given me some fascinating insights into a long-time Rubyist's transition into Elixir. The baggage Ruby developers bring with them when they come to Elixir, how it shapes a code base, and ultimately how it can be avoided for newcomers. 

From working in both codebases I have seen the dangers of what I call "rebuilding Rails".  In the quest to recreate the familiar feel of Ruby and Rails, it's easy create bad patterns, overuse macros, create unnecessary convenience functions  and attempt to create an object-oriented language inside a functional one. I will be diving into patterns I discovered, eventually refactoring many of them (sometimes painfully).

How can we soften the landing for new Ruby developers? How can these patterns, once adopted, be refactored and adjusted to a more idiomatic Elixir approach? In doing so I think we can make the language more welcoming, set projects and developers up for long term success and create robust projects.

**Key Takeaways:**

- My aim with this talk is two fold: both general interest for those who looking to compare the evolution of real-world codebases as a team grew their Elixir skills and more importantly, to help experienced Elixir developers create a softer landing for incoming Ruby developers. I believe this will not only create fewer headaches when hiring from the Ruby world but will also aid adoption of Elixir in an existing Ruby team.
