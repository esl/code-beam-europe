---
tags:	
- neural network inference, lightweight, edge device
level: Intermediate
title: 	"TFLiteBEAM: Empowering Edge Devices with Lightweight Neural Network Inference Framework"
speakers:
- _participants/cocoa-xu.md

---
This project aims to create a lightweight neural network inference library, TFLiteBEAM, powered by TensorFlow Lite (TFLite).

Firstly, TFLiteBEAM has a small footprint. It sits around 10MBs compared to 500+ MBs when using EXLA or 700+ MBs for torchx, making it a great option for edge devices and resource-constrained systems such as Raspberry Pi.

Secondly, TFLiteBEAM is primarily optimised for mobile and embedded devices. It provides optimized model parsers and inference engines for these devices, delivering fast and low-latency inference performance.

Thirdly, using TFLiteBEAM also allows us to run models on Edge TPU like Coral, a hardware accelerator. In comparison, it's still nearly impossible to use any desktop GPUs on devices like Raspberry Pi, while adding a Coral edge TPU as the hardware accelerator is relatively more accessible and practical.

Lastly, as its name suggests, this library can benefit all BEAM languages (as long as they have support for using Erlang NIF libraries).

**Target Audience:**
- Anyone who's interested in a neural network inference library for edge/mobile/embedded devices like Raspberry Pi.
