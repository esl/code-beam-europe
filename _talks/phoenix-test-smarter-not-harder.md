---
tags: tests liveview wallaby
level: Intermediate
title: "Phoenix: Test smarter, not harder"
speakers: -_participants/fredrik-teschke.md

---
Have these thoughts crossed your mind?_x000D_
_x000D_
- "Feature tests are just too much work."_x000D_
- "Oh no! Converting this dead view into a live view means I'll have to delete or rewrite all the tests."_x000D_
- "From a UX perspective, this should be implemented with Javascript. But then I would have to rewrite all my tests. Nah, I'll do a full handle_event roundtrip instead."_x000D_
_x000D_
If so, this talk is for you! We will:_x000D_
_x000D_
1. explore the current testing landscape for Phoenix_x000D_
2. compare it to other ecosystems (Ruby, Javascript, Java)_x000D_
3. discuss what could be improved (for Phoenix)_x000D_
4. give a quick intro to phoenix_test, the new kid on the block_x000D_
5. see how to test Javascript-reliant views, without having to rewrite the tests

**Key Takeaways:**
- comparison of end to end testing alternatives: Wallaby and playwright (used by phoenix_live_view)_x000D_
- LiveView testing is already pretty good compared to other ecosystems (batteries included to write performant and expressive tests)_x000D_
- there's a gap between the test API's depending on view implementation: 1. dead views, 2. live views and 3. Javascript-reliant views_x000D_
- when switching the view implementation, tests have to be rewritten_x000D_
- this could be solved by writing all tests as browser based tests (Wallaby)_x000D_
- but that's not ideal: long execution duration (cost in CI, developer experience)_x000D_
- phoenix_test bridges the testing gap between dead and live views_x000D_
- a browser-based plug-and-play driver for phoenix_test (e.g. Wallaby) allows you to keep your tests when switching view implementation_x000D_
- phoenix_test provides a descriptive API for writing feature tests

**Target Audience:**
- Web developers (all experience levels)

