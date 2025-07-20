---
tags: 
  - DNS
  - scalability
  - extensibility

level: Intermediate
title: "Scaling, securing, and protecting DNS, in Erlang"
speakers: 
  - _participants/nelson-vides.md

---
DNS is that protocol we all seem to know the basics of it but we all know we don’t know it in depth. It is at the core of the internet and we all need it to work, but, how does it work? And maybe more interestingly, how does it not work? And how is it implemented?
This presentation explores the application of Erlang/OTP in a DNS nameserver, highlighting its strengths and weaknesses, and the trade-offs. We’ll also compare against leading C++ solutions, judging by performance, fault-tolerance, development ease, and community support. We’ll cover engaging challenges, like:
- How to implement a Plug-inspired extensible protocol: a purely functional idiom that allows for easy extensibility and testing
- Networking stack in the BEAM: a critical component of any server and how to it tailor to your needs
- DNSSEC and proof-of-non-existence: at scale, what do you sign, an empty string?!
- Surviving DDoS attacks: did you know DNS DDoS represents a quarter of the world’s DDoS attacks?
- What’s next: how I think the future will look for DNS and the BEAM

**Key Takeaways:**
- A text-book example of the BEAM's best features.
- Insights into DNS operations and the strengths/weaknesses of Erlang/OTP for DNS.
- Comparative analysis of Erlang/OTP and C++ solutions, focusing on performance and security.
- Future trends in DNS and strategies for handling challenges like DDoS attacks.

**Target Audience:**
- Developers curious about how such a core component of the internet is implemented in a functional and concurrent paradigm.
- Professionals seeking advanced insights into DNS implementation and security.
- Anybody looking for a perfect text-book example of Erlang's programming model, including supervision trees, networking capabilities, concurrency, fault-tolerance, light-weight processes, ets tables, you name it.
