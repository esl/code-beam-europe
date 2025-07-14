---
tags: 
  - vision
  - elixir
  - yolo

level: Intermediate
title: "Teaching the BEAM to See"
speakers: 
  - _participants/alvise-susmel.md

---
What if your Elixir application could see and understand the world around it? In this talk, we'll explore how to bring state-of-the-art object detection and tracking directly into your Elixir applications.

I'll demystify how YOLO models work and show you how to integrate both Ultralytics and YOLOX models (including custom-trained ones) into Elixir using the YOLO library. We'll briefly explore how to train a model on your custom data and dive into the mechanics of object detection and tracking, understanding how to maintain consistent identities as objects move through your camera's view.

Through live demos, you'll see how to build responsive pipelines with accelerated inference and benchmark them on edge devices. Building on Paulo Valente and Vittoria Bitton’s work running inference on a Raspberry Pi 5 with the Hailo-8 AI Hat, we'll explore performance across various edge devices and hardware acceleration options. Whether you're building IoT applications or interactive experiences, this talk will show you how to give your BEAM applications the gift of sight while leveraging Elixir's concurrent, fault-tolerant architecture.

**Key Takeaways:**

- Understand how YOLO models work under the hood and how to integrate them into Elixir applications using the Elixir YOLO library.
- Learn the fundamentals of object detection and tracking, including how to maintain consistent object identities across video frames.
- Discover how to use both pre-trained and custom-trained models, with a brief overview of training on your own data.
- Gain insights into edge device performance and deployment considerations for computer vision workloads.

**Target Audience:**

- Elixir developers curious about AI/ML integration, IoT enthusiasts working with embedded systems and edge devices, developers interested in real-time computer vision applications, and anyone looking to add intelligent visual capabilities to their BEAM-based projects.
