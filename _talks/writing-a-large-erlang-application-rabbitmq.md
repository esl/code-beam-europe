---
audience:
- Intermediate
tags:
  - Exciting RabbitMQ Core
title: "Writing a large Erlang application: RabbitMQ"
speakers:
- _participants/iliia-khaprov.md

---
RabbitMQ project touches all aspects of development - from user stories to writing code to delivering OS-specific packages.

In this talk we will learn about RabbitMQ development pipeline, as well as its architecture.

In particular we will focus on recently introduced so-called native protocol rewrites. Respective protocols (MQTT & AMQP1.0) now use much more granular and low-level primitives of the RabbitMQ Core API. In this session, we will explore these APIs as well as review what could be seen as a template for RabbitMQ protocol implementation.