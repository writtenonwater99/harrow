# Harrow

**Open-source release in preparation.** This repository is the reserved public home for the open half of Harrow. It exists so the commitment is public before the release is.

## What Harrow is

A payer's record of itself lives in fragments spread across other people's systems: claims with one vendor, eligibility with another, prior years with a contractor whose contract has ended. Harrow brings those fragments together over the systems already running, inside a boundary the payer or its sponsor controls.

It keeps each fragment as it arrived. Where two sources disagree, both values stay, each with its origin. Nothing is picked as the winner in storage. When a use needs one value, it picks by a named rule, and the pick is recorded. Every value carries the evidence behind it: the source it came from, what changed on the way, and a hash over the source bytes.

## What will be open

A receipt that only its vendor can check is not much of a receipt. The parts a payer needs to check Harrow's output independently will be published under the ZKEL standard:

- The record shapes
- The lineage and provenance model
- The receipt format and its verification algorithm
- Conformance tests and a reference verifier

The aim is that anyone who holds a record and its receipt can recompute the receipt themselves, without asking us.

## What stays commercial

The refinery stays commercial: the adapter library, the reconciliation rules, how records are matched across sources, and the merge pipeline. The standard describes what a conformant record and receipt look like. How we produce them is our work.

## Why this is public now

The record lives inside the payer's own boundary, in an open shape. Once the standard and verifier are released, the payer keeps all three even if we disappear: the record, the standard, and the verifier. Publishing the commitment before the code is how that promise starts.

## Until release

Harrow is built by [Zkeleton](https://zkeleton.com). The product page is at [zkeleton.com/harrow](https://www.zkeleton.com/harrow).
