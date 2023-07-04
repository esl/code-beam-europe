---
tags:	
- state-machine, legacy-firefighting, technical-debt
level: Intermediate
title: 	"Reimplementing Technical Debt with State Machines"
speakers: _participants/nelson-vides.md
		  _participants/pawel-chrzaszcz.md

---
An extensible protocol implementation means that its core code has to be extensible, right? But it also means the core is the first piece of code ever written for this project, and which everything else will depend on, which means, well, highly likely future technical debt.
Fast-forward over a decade, and this code might have become not just intractable, but also impossible to understand. What's next? Incremental improvements, top-bottom or bottom-up, a full rewrite and replug, experiment with a mysterious and not fully tested spaghetti?
In our chat’s backend service, we kept coming back to this topic, until one day that looked like it’d be just a boring day, we came up with a prototype for a remorseless full rewrite that immediately looked promising. Based on the OTP’s gen_statem behaviour, we wrote a new core set of extensible rules where everything can gracefully plug in.
Let's solve the quagmire putting together old code, RFCs, state machines and a telemetry-like event mechanism.

**Key Takeaways:**
All the bells and whistles OTP's gen_statem has to offer, which is often the right tool for the job and just as often a tool forgotten about. A set of ideas on how to make a core protocol meant to be extensible implemented and stable.

**Target audience:**
- Legacy-code firefighters as well as people implementing extensible protocols from scratch.