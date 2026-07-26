## Max Friedman

Product Manager on **Gemini Intelligence & Pixel AI** at Google, working on the
part of assistance that isn't the model: deciding what a device should surface,
when it should stay quiet, and how much of the reasoning can happen on the phone
instead of in a datacenter.

Before this — Google Shopping APM, co-founder and co-CEO of a bootstrapped
athlete-monetization marketplace, and a stint modernizing satellite data
pipelines at NASA JPL. USC, CS + Business Administration.

I write code as a PM, not instead of engineers. Most of what's here is me
building the thing to find out whether the idea survives contact with an
implementation.

---

### Currently building

**[tactbench](https://github.com/max-friedman/tactbench)** — a benchmark for
whether an assistant should speak at all.

Nearly every LLM eval asks *how good is the answer*. Proactive assistants face a
prior question nobody scores: **should you have said anything?** That's not
accuracy — the costs are asymmetric and depend on what the user was doing.
Interrupting deep work isn't the same mistake as interrupting someone in line for
coffee, and neither is waking them at 3am.

The result that makes the case: a policy that surfaces *everything* achieves
**perfect recall** and still scores 165 points **worse than saying nothing at
all**. Optimize for helpfulness and that's where you land.

Python · asymmetric cost scoring · adversarial matched-pair dataset · local viewer

---

### How I work

- **Benchmarks before opinions.** If I'm claiming a product judgment is hard, I'd
  rather ship the eval that proves it than argue about it in a doc.
- **Ship the limitations section.** Every repo here states what it doesn't yet
  measure. A benchmark that overclaims is worse than no benchmark.
- **Agentic loops.** Most of this is built with Claude Code driving long
  iteration cycles — roast, prioritize, implement, verify, repeat.

### Elsewhere

[LinkedIn](https://linkedin.com/in/maxhfriedman)
