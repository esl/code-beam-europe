---
tags:
  - OTP Lustre Fullstack

level: Intermediate
title: "Asterism: An OTP Visualizer in Gleam"
speakers:
- _participants/guillaume-heu.md
published: true

---
With the goal of understanding OTP better, I started working on a BEAM process graph visualizer. After many tangents, I built Asterism, a web application that presents a BEAM node's process graph and application trees. Using a BEAM web server and a Javascript client with Lustre, I fully leveraged Gleam's multi-target capabilities  to make a reusable full-stack OTP display with a single language (that isn't Typescript.)
In this talk, I take the audience through my journey, discovering the structure of OTP applications, learning how to create and lay out graphs, and many web development side-quests with Gleam, Mist and Lustre.

**Key Takeaways:**

- Gleam tooling for OTP is growing more and more robust. Gleam is also a bridge between back-end and front-end development. The components offered by the Lustre web framework make reusing and integrating entire webapps trivial.

**Target Audience:**

- Anyone looking to learn about Lustre and server components, interested in making graphs with Lustre, or looking for a narrative introduction to OTP.
