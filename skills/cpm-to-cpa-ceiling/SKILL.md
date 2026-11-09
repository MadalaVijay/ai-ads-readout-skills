---
name: cpm-to-cpa-ceiling
description: Turn a cost per thousand impressions into the cost per customer it implies, and the click and conversion rates that would be needed to break even. Use when a surface bills on impressions and someone needs to know whether the price can ever work.
---

# From CPM to a cost per customer

A surface that bills per thousand impressions does not tell you what a customer
costs. Three rates sit between the two, and **a price that looks high can be
affordable and a price that looks low can be hopeless** depending on them.

## The chain

```
cost per customer = CPM / 1000
                    / click rate
                    / conversion rate per click
```

Cost per impression, divided by the share who click, divided by the share of
clickers who become customers. Every term is a ratio you can estimate, and
every one can move the answer by a large multiple.

## Start from the ceiling, not the price

Work backwards. Take the most you can pay for a customer and still be
profitable, then ask what the other two terms would need to be:

```
required click rate = CPM / 1000 / ceiling / conversion rate per click
```

If the required click rate is far above anything the surface plausibly delivers,
the channel cannot work at that price and no creative will change that. If it is
well within reach, the question becomes whether you can get there.

## Use your own conversion rate, not the surface's

Your conversion rate per click comes from your page and your offer. Take it from
your own traffic of a similar intent level, and be cautious about assuming
visitors from a new surface convert like visitors from search. They arrive in a
different frame of mind. Treat the borrowed rate as a guess and give a range.

## Run it as a range

Build a small table, not one answer. Three click rates, three conversion rates,
nine outcome costs, with your ceiling marked. The shape matters more than any
cell:

- If every cell is above the ceiling, the price is the problem.
- If every cell is below it, the risk is volume, not price.
- If it straddles, the click rate and conversion rate are what you are really
  testing, and the test should be built to measure those two.

## Include what the CPM leaves out

Check for costs outside the quoted rate: platform fees, minimum commitments,
creative production, the time to manage a new channel. A price that clears the
ceiling before those and fails after is a fail.

Also check whether the billing is per impression or per click. A click-billed
campaign has no CPM term, and the chain collapses to cost per click divided by
conversion rate.

## Do not use a quoted price as an estimate for your own

Prices on auction-based surfaces move with demand, targeting and time. A figure
from an article is a pointer to the order of magnitude. Your own invoiced cost
after a small test is the number to use.

## Output

The ceiling and where it came from. The three rates with the range used for each
and the source of each. The sensitivity table with the ceiling marked. Whether
the price is the problem, the volume is the risk, or the click and conversion
rates are the open question.

## What this does not cover

How big a test to run to measure those rates, see `new-surface-test-budget`.
Deciding the verdict, see `no-benchmark-verdict`. How the ceiling relates to
lifetime value, which is a unit-economics question.
