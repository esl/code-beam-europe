---
tags:
  - erlang
  - tracing
  - debugging

level: Intermediate
title: "Making Your System Debuggable - Lessons from Erlang Doctor"
speakers:
- _participants/pawel-chrzaszcz.md
published: true

---
After years of building custom tracing tools to debug complex Erlang systems, in 2017 I decided to make them reusable and public as erlang_doctor, followed by its Elixir counterpart, ex_doctor. Debugging issues in complex Erlang systems such as MongooseIM was a real-world battlefield for me, where I refined the tools over the years with the help of suggestions from my colleagues at Erlang Solutions. Their current versions allow extensive tracing with minimal impact on the running system, and querying the collected data afterwards.

In this talk, I will show real-life examples of diagnosing elusive and subtle issues. Such experiences allowed me not only to keep improving the tools, but also to make my own code easier to debug, and - in a broader sense - easier to reason about. Are there any coding practices that could make you get rid of a bug in a matter of minutes rather than days? Or maybe there are some anti-patterns to avoid? And how do tracing, instrumentation, logging and metrics complement one another? These questions are not easy to answer, but I will share practical insights that can help you improve your own Erlang system.

**Key Takeaways:**

- How and when to use Erlang Doctor to speed up tracing/debugging.
- How to improve their own code to make it easier to debug and comprehend.

**Target Audience:**

- Erlang/Elixir engineers facing the reality - software with bugs, most of them difficult to find, especially if the system is complex
