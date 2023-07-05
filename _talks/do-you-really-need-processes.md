---
tags:	
- Processes, Design, Exploration
level: Intermediate
title: 	"Do You Really Need Processes?"
speakers:
- _participants/brian-underwood.md

---
You probably know that the power of the BEAM comes from processes which operate concurrently and supervisors which, in many cases, allow service to continue.  Maybe you’ve thought that your application needs to use more GenServers and Supervisors to become the best that it can be.  But then again, maybe everything is fine.

In this talk, Brian will present a demo of a ride-sharing application which he created to understand what is possible with a standard Phoenix + PostgreSQL application. He will explore what performance and resiliency gains can (or can’t)  be achieved by designing various process and supervision architectures using an external database, process state, ETS tables, and combinations therein.

**Key Takeaways:**
- How to think through the process of designing GenServers and supervisors
- Not using processes is a valid solution much of the time
- Understanding of what’s possible with the BEAM and gaining an appreciation for what’s involved

**Target Audience:**
- Elixir developers who understand some of the basic concepts but don’t yet fully understand how to think through the pros and cons of designing for processes. 