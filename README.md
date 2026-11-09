# ai-ads-readout-skills

Claude Code skills for reading the results of a new ad surface when there is no
benchmark to read them against: conversational ads, AI-answer ads, and whatever
launches next.

Not a platform guide. Not campaign setup. These skills start when you already
have numbers and no way to tell whether they are good.

## The problem this repo rests on

On a new surface, the first thing everyone asks is "what is a good CTR?" and the
honest answer is that nobody knows yet. Published figures come from a few
advertisers or one agency's clients, are often unsourced, use different
definitions, and disagree with each other. Platforms may say outright that they
have no cross-advertiser benchmarks.

So teams do one of two things. They borrow a number from an article and plan
around it, or they judge the surface by comparing its CTR to search, where the
click means something different. **Both produce confident decisions on
evidence that cannot support them.**

These skills encode the alternative: define success from your own economics,
judge on outcome cost rather than intermediate metrics, and refuse a verdict
when the data cannot give one.

## The six skills

```
skills/
  no-benchmark-verdict/     continue, stop, or cannot tell yet, from your own numbers
  benchmark-provenance/     where a quoted figure came from, and how many origins it has
  low-ctr-quality-read/     what a low click rate means, and what the few clicks did
  cpm-to-cpa-ceiling/       whether an impression price can ever pay for a customer
  new-surface-test-budget/  how much to spend to find out, and when to stop
  halo-and-spillover/       testing the "it helps elsewhere" claim without fooling yourself
```

## Start here

| What you are doing | Skill |
|---|---|
| Someone asks "is this CTR or CPM good?" | `no-benchmark-verdict` |
| A deck or article quotes a benchmark | `benchmark-provenance` |
| Clicks look low next to search | `low-ctr-quality-read` |
| Impression-billed and unsure it can pay | `cpm-to-cpa-ceiling` |
| Planning a first test | `new-surface-test-budget`, then `cpm-to-cpa-ceiling` |
| "It is helping, just not in the report" | `halo-and-spillover` |

**Work out your ceiling first (`cpm-to-cpa-ceiling`).** Every other judgment here
needs a number you would call good, and it has to come from your economics, not
from a post.

## Install

```bash
git clone https://github.com/MadalaVijay/ai-ads-readout-skills
cp -r ai-ads-readout-skills/skills/* your-project/.claude/skills/
```

## The ideas these keep returning to

**A benchmark with no traceable owner is not a benchmark.** Count origins, not
citations: ten articles can share one source.

**Judge on cost per customer, not on CTR, CPM or CPC.** Those describe how a
surface behaves, not whether it pays.

**"Cannot tell yet" is a real verdict,** provided it comes with the result count
at which you will decide. Without that it just means "keep spending."

**Write the continue and stop numbers before the money goes out.** After the
results arrive they set the target quietly.

**A halo claim is a hypothesis to test, not a reason to keep paying.** Name the
signals in advance, check the timing, rule out what else changed.

**A first-week result on a surface that is still changing is a date-stamped
observation,** not a finding. Re-test before scaling.

## Prior art

For operating a specific platform end to end, including setup, policy and
platform behaviour,
[AI-Marketing-Hub/chatgpt-ads](https://github.com/AI-Marketing-Hub/chatgpt-ads)
is a sourced knowledge and skill pack for ChatGPT Ads. For breadth across
marketing in general,
[coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills).
For broad multi-platform paid media,
[AgriciDaniel/claude-ads](https://github.com/AgriciDaniel/claude-ads). This repo
is deliberately narrower: it is about judging the numbers, on any new surface,
and it complements those rather than replacing them.

## What this does not cover

- Platform setup, campaign structure, creative specs and policy
- Specific platform behaviour, which changes quickly and is better read from live
  documentation than from a repository
- Statistical testing and power calculations
- Running a holdout or geo-holdout test; `halo-and-spillover` only decides
  whether the claim is worth one
- Tracking implementation and conversion-API setup
- Any claim about what a given surface currently costs or delivers. These skills
  deliberately contain no benchmark figures

## Notes

Written from running paid acquisition across several channels and from the
repeated experience of watching a number from a post become a target.

Conventions here, such as the ten-result floor, are starting points. Tune them to
your volumes and your cost of being wrong.

MIT licensed. Issues and corrections welcome.
