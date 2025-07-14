---
tags:
  - Riak Search
  - OpenRIak
  - VMs

level: Intermediate
title: "Why We Killed Riak Search, and What We Are Doing Instead"
speakers:
  - _participants/nicholas-adams.md
  - _participants/peter-clark.md
---
Riak Search was a Solr-based full-text search engine included in Riak KV. This talk is about why it wasn't a good idea, and what we are planning to replace it. We'll discuss the issues we found when trying to manage a Java VM from the Erlang VM, scaling issues encountered, and how people got around them. We'll also touch on how to do searches at the moment in OpenRiak KV 3.2.5 using secondary indexes and regular expressions, and discuss the new Filters-based search in OpenRiak KV 3.4. We'll finish with how to integrate 3rd party search engines such as OpenSearch using the TicTac reconciliation engine.

**Key Takeaways:**

- Why not to use multiple VMs on the same box, how to spot when this is an issue, how OpenRiak dealt with this, and how OpenRiak brought back similar functionality in a better way

**Target Audience:**

- Anyone whose code relies on a 3rd party VM such as Java
