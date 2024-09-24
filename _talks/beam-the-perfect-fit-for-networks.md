---
tags:	
- networking low-level programming 
level: Intermediate
title: 	"BEAM: The Perfect Fit for Networks"
speakers:

---
Networking can seem like a challenging task, but the BEAM is truly one of the best matches for tackling it. In this talk, we’ll mostly focus on two things: when the BEAM is the right fit for networking applications, especially compared to “lower-level” languages (such as Rust or Go), and then we’ll shift our focus to using the BEAM to write TCP applications.

- We'll discuss how the BEAM's lightweight processes and messaging system provide a powerful and intuitive way to handle TCP sockets and data.
- We'll explore how to use acceptor pools and supervision trees to build scalable and fault-tolerant TCP servers.
- I’ll show you how to use the gen_statem behaviour to build reliable TCP clients.

This stuff is at the foundation of Phoenix, LiveView, channels, and more. Even if you’re not working at the lower levels of the networking stack, this talk will help you understand how many of the tools and patterns we use every day work under the hood.

**Key Takeaways:**
- The BEAM is a fantastic fit for networking
- The process model used by the BEAM mirrors how networks of computers behave.
- The BEAM includes many tools to make working with networks easy, pleasant.
- Network systems built on the BEAM are relatively-easy to make resilient and scalable.

**Target Audience:**
- Folks that are familiar with the basics of network programming, as well as folks familiar with the BEAM who are interested in how it fits the network programming use case.