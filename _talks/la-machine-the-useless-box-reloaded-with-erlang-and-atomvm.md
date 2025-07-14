---
tags: "La Machine in Erlang"
level: Introductory and overview
title: "La Machine: The Useless Box reloaded with Erlang and AtomVM"
speakers: -_participants/paul-guyot.md
published: false
---
Why and how Erlang and AtomVM were used to develop the personality of a lovable IoT device while maximizing its battery life.

Session will include video demos of La Machine (https://la-machine.fr/) and most importantly the Erlang journey towards the product:
- hardware prototyping including a small ESP32c3 board powering it
- usage of rebar3 to flash Erlang code on it
- usage of console
- usage of AtomVM API for GPIO and servo (PWM)
- usage of CI with dialyzer and tests, including qemu
- specific AtomVM API for ESP32 deep sleep
- how a C library was ported as an AtomVM NIF for audio decoding, with a glimpse on AtomVM SMP builds (even if ESP32C3 is single core)
- quick overview of memory management on AtomVM

**Key Takeaways:**
- How to use AtomVM to prototype and build IoT devices using Erlang or Elixir.
- This includes using existing libraries (GPIO, PWM will be explicitely mentioned, but I2C is straightfoward), as well as porting more complex ESP32 component libraries as NIFs.

**Target Audience:**
- Erlang developers
- Elixir developers
- IoT enthusiasts and hackers
