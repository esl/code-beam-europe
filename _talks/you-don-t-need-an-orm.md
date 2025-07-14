---
tags: 
  - postgres
  - sql
  - database

level: Introductory and overview
title: "You Don't Need an ORM"
speakers: 
  - _participants/giacomo-cavalieri.md

---
Using SQL from other programming languages can prove to be quite the hassle: wrangling the database rows into the host's language types is tedious and error prone, and making sure the application code stays up to date with the ever-changing database schema is just as challenging.

To address these developer experience shortcomings ORMs try to shield the developer from ever having to write any SQL at all.  This doesn't feel totally satisfying though: as developers we are always keen on using the right language for the job, so what would it look like to fully embrace SQL instead of trying to abstract it away? 

In this talk we'll look at Squirrel, a library that tackles database access in Gleam: a functional, statically-typed language. We'll explore how code generation from raw SQL can help bridge the gap between the database and a functional language without compromising on type-safety, performance or developer experience.

**Key Takeaways:**

- This talk will show you how one can use the right language for the job when faced with the task of talking to a database. As it turns out, we can stick to writing “plain old SQL” without having to resort to fancy (and leaky!) abstraction or compromising on developer experience!

- You'll discover how one can embrace SQL while using the functional languages they know and love, and what a fun time this can be!

**Target Audience:**

- This talk is for everyone! You might  find it particularly interesting if:
- you have ever had to debug a nasty N+1 query problem, or an ORM performance issue, and wondered “is there a different way?”
- if you are curious to learn how one can stick to plain old SQL and still have a good time using their favourite language of choice for app development
