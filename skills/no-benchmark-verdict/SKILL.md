---
name: no-benchmark-verdict
description: Decide whether a new ad surface is working when no industry benchmark exists. Use when someone asks "is this CTR or CPM good?" about a channel that launched recently, or when a campaign has results but nothing to compare them to.
---

# Verdict without a benchmark

On a new ad surface the question "is this good?" has no external answer yet.
Published numbers are a handful of advertisers and agencies, mostly unsourced,
and they disagree with each other. Do not borrow one. **The only valid baseline
is your own business.**

## Define good before the money is spent

Write down, before launch, the single number that would make you keep going and
the single number that would make you stop. Both come from your own economics:

- The most you can pay for a customer and still be profitable. See `cpm-to-cpa-ceiling`.
- What your next-best channel currently costs for the same outcome.

If these are written after the results arrive, the results will quietly set them.

## Compare on the outcome, never on the intermediate metric

CTR, CPM and CPC are properties of how a surface works, not of whether it pays.
A surface can have a low click rate and a cheap customer, or a high click rate
and a worthless one. Judge on cost per acquired customer, or the nearest
honest stand-in when volume is too thin.

Compare against **your own other channel measured the same way, over the same
window, with the same conversion definition.** If the definitions differ, the
comparison is noise.

## The three verdicts

Pick exactly one. "Promising" is not a verdict.

**Continue.** The outcome cost is inside your ceiling, or on a trajectory to
be, and enough results exist to believe it. State the number that would flip it.

**Stop.** The outcome cost is outside your ceiling with enough results that more
spend is unlikely to change that. Stop is a real answer, not a failure.

**Cannot tell yet.** Too few results to say. This is a legitimate verdict and
should come with the exact count of results or the spend at which you will
decide, written down now. Without that, "cannot tell yet" becomes "keep
spending."

## The minimum before any verdict

Below roughly ten attributed results, an outcome cost is mostly noise: one more
or one fewer result moves it by a large fraction. Report the count next to every
cost figure, and refuse a Continue or Stop below your floor. Tune the floor to
your situation; ten is a convention, not a law.

## Watch the one failure that is specific to new surfaces

Early results are often unrepresentative because the surface is changing under
you: formats, targeting options and measurement all get revised while you are
testing. A result from the first weeks may not describe the surface a quarter
later. Date every finding and re-test before scaling on it.

## Output

The pre-written continue and stop numbers. The outcome cost against your
comparison channel, with both result counts. One verdict from the three. If
"cannot tell yet", the exact trigger for deciding. The date, so the finding can
be recognised as stale.

## What this does not cover

Where a quoted benchmark came from, see `benchmark-provenance`. Working out the
ceiling itself, see `cpm-to-cpa-ceiling`. How to run the test, see
`new-surface-test-budget`.
