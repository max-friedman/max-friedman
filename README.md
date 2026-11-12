## Max Friedman

PM on **Gemini Intelligence & Pixel AI** at Google, working on the part of
assistance that isn't the model: deciding what a device should surface, when it
should stay quiet, and how much of the reasoning can happen on the phone instead
of in a datacenter.

I build the prototype before I write the doc. Everything here started as a
product question I couldn't settle by arguing about it.

Before this: Google Shopping APM, co-founder and co-CEO of a bootstrapped
athlete-monetization marketplace, and modernizing satellite data pipelines at
NASA JPL. USC, CS + Business Administration.

---

### Built from zero

**[tactbench](https://github.com/max-friedman/tactbench)**: a benchmark for
whether an assistant should speak at all. Proactive assistants face a question
no common eval scores: *should you have said anything?* A policy that surfaces
everything gets **perfect recall** and still costs **294 points more than saying
nothing at all**. Shortcut resistance is measured, not claimed: keyword and
bigram probes sit at chance on held-out phrasings.
`Python · asymmetric cost metric · matched-pair dataset · CI-checked results`

**[agentic-coding-loop](https://github.com/max-friedman/agentic-coding-loop)**:
a protocol that lets a coding agent improve a codebase over weeks of sessions
that start with no memory, plus governance so the protocol can't be quietly
weakened. Its first audit round caught a false claim tactbench had shipped since
its first commit (the probe hit 93.5% against a 50% floor). A predecessor ran
120+ rounds on a live consumer app. Installs as a Claude Code plugin.
`Claude Code plugin · state-file spine · reject-by-default review`

### Upstream

Root-caused bug reports in
[NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent):
gateway freezes from full GC on macOS, hook context leaking into memory review,
and a launchd restart that never recovers.

### How I work

- **Benchmarks before opinions.** If I'm claiming a product judgment is hard,
  I'd rather ship the eval that proves it than argue about it in a doc.
- **Ship the limitations section.** Every repo here states what it doesn't yet
  measure. A benchmark that overclaims is worse than no benchmark.
- **Agents run the long loops.** Most of this is built with Claude Code driving
  multi-week iteration cycles: roast, prioritize, implement, verify, repeat.

### Elsewhere

[LinkedIn](https://www.linkedin.com/in/maxhfriedman/)
