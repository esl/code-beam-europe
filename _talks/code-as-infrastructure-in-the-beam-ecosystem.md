---
tags:	
- Erlang, devops, learnings
level: Intermediate
title: 	"Code as infrastructure in the BEAM ecosystem"
speakers: 
- _participants/jade-allen.md

---
Building applications in the BEAM ecosystem is generally a good developer experience, but dealing with the packaging, deployment and configuration of those applications into operational environments has few best practices and often leads to ad-hoc and manual processes which are fine for small deployments - but completely inadequate for managing a fleet of servers. In this talk, I will share many of the lessons I learned building Erlang releases for both Debian installations and minimally small Docker containers - and how we used ansible to script application configuration, software upgrades and automated deployments into various environments.

**Key Takeaways:**
- Learn how to:
* Build minimally small Erlang Docker containers for your application releases,
* Script application configuration using tools like ansible
* Manage application upgrades across fleets of infrastructure

**Target audience:**
- People who want to manage BEAM applications running on large sets of infrastructure.