---
tags:	
- multiplayer-tetris, elixir, case-study
level: Intermediate
title: 	"Let’s play Tetris together! - Building Multiplayer Tetris from scratch with OTP, Elixir, and Phoenix"
speakers:
- _participants/merlin-webster.md

---
Let’s play Tetris together!

In this talk we’ll play a live game of Tetris battles together, and then have a look at how it works under the hood. We’ll take a tour through the code and show how a multi-participant browser based game or tool can be built using only Elixir and Phoenix LiveView.

The goal of this talk is to teach you something about how OTP processes and supervision works, and show some patterns for creating large interactive experiences using Phoenix.

We’ll use my game <a href="https://github.com/mjftw/Tetrex"> Tetrex </a> as a case study, and I’ll aim to share some insights learned on my journey from Elixir newbie to video game copyright infringer.

**Key Takeaways:**
- What does the talk aim to achieve?
* To show some patterns for building resilient and scalable multiplayer applications using Elixir, Phoenix LiveView and PubSub. …and hopefully have a bit of fun along the way!
- What will the audience learn?
* How to spin up and supervise many OTP processes that work together to do something interesting.

**Target Audience:**
- Elixir developers who want to learn more about OTP processes and Phoenix LiveView to build games and other online multi-participant applications.
- The talk is aimed at those who know a bit of Elixir, but are unsure how to bring all the various elements like OTP & Phoenix together to build a complex system.
- Anyone who likes retro video games.