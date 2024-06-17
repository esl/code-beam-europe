---
tags: 
  - tests
  - liveview
  - wallaby
level: Intermediate
title: "Phoenix: Test smarter, not harder"
speakers: -_participants/fredrik-teschke.md

---
Have these thoughts crossed your mind?

- "Feature tests are just too much work."
- "Oh no! Converting this dead view into a live view means I'll have to delete or rewrite all the tests."
- "From a UX perspective, this should be implemented with Javascript. But then I would have to rewrite all my tests. Nah, I'll do a full handle_event roundtrip instead."

If so, this talk is for you! We will:

1. explore the current testing landscape for Phoenix
2. compare it to other ecosystems (Ruby, Javascript, Java)
3. discuss what could be improved (for Phoenix)
4. give a quick intro to phoenix_test, the new kid on the block
5. see how to test Javascript-reliant views, without having to rewrite the tests

**Key Takeaways:**
- comparison of end to end testing alternatives: Wallaby and playwright (used by phoenix_live_view)
- LiveView testing is already pretty good compared to other ecosystems (batteries included to write performant and expressive tests)
- there's a gap between the test API's depending on view implementation: 1. dead views, 2. live views and 3. Javascript-reliant views
- when switching the view implementation, tests have to be rewritten
- this could be solved by writing all tests as browser based tests (Wallaby)
- but that's not ideal: long execution duration (cost in CI, developer experience)
- phoenix_test bridges the testing gap between dead and live views
- a browser-based plug-and-play driver for phoenix_test (e.g. Wallaby) allows you to keep your tests when switching view implementation
- phoenix_test provides a descriptive API for writing feature tests

**Target Audience:**
- Web developers (all experience levels)

