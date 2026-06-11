---
tags:
  - BEAM
  - distribution
  - libcluster

level: Intermediate
title: "ClusterFu**tional: Four Years of Distributed Elixir at NetzeBW"
speakers:
- _participants/aaron-cruz.md
published: true

---
Clustering is one of the BEAM's best selling points and one of its least understood. Most of us learn just enough to get nodes talking and then close our editor, which is a shame, because the interesting stuff starts right after that.

Distribution on the BEAM isn't a library bolted on top, it's baked into the runtime. Once you understand what it's actually giving you, a lot of the things you'd normally reach for (queues, RPC layers, service meshes) start to look like workarounds for problems you don't have.

I'll cover how nodes find each other, how processes get spread across a cluster, and what libcluster is actually doing under the hood, plus the patterns that hold up in production and the drawbacks nobody warns you about. I'll also get into when distributed Erlang is the right tool and when you should pick something else instead, because the answer isn't always "cluster it."

All of it drawn from 4+ years building NETZlive at NetzeBW, where we help coordinate the German power grid.

**Key Takeaways:**

- how the BEAM does distribution under the hood
- patterns that work in production
- handling net splits (service is down)
- the drawbacks nobody warns you about

**Target Audience:**

- devs who've only ever done cross-service communication over HTTP
- people curious how distribution works deeper in the stack
- anyone running services in Kubernetes or similar
