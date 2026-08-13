# Harrow

**Open-source release in preparation.** This repository is the reserved public home for the open half of Harrow. This page exists so the commitment is public before the release is.

## What Harrow is

Harrow is a payer-owned truth layer. A payer's record of itself lives in fragments spread across other people's systems: claims with one vendor, eligibility with another, prior years with a contractor whose contract has ended. Harrow reconciles those fragments into one lineage-complete, receipted record, over the systems already running, inside a boundary the payer or its sponsor controls. Every merged value carries the evidence that produced it: the rule that decided, the raw source bytes the value came from, and a hash over those bytes.

## What will be open

A receipt that only its vendor can check is not evidence. The parts of Harrow a payer needs to verify its output independently are published under the ZKEL standard:

- The record shapes
- The lineage and provenance model
- The receipt format and its verification algorithm
- Conformance tests and a reference verifier

With these published, a payer, a regulator, or an auditor can recompute any receipt from the record it describes, without asking us.

## What stays commercial

The refinery stays commercial: the adapter library, the reconciliation rulesets, how records are matched across sources, and the merge pipeline. The standard says what a conformant record and receipt look like. How we produce them is our work.

## Why this is public now

The record lives in the payer's own boundary, in an open shape, with an open verifier. If Harrow the company disappeared, the record, the standard, and the verifier would remain with the payer. Publishing the commitment before the code is how that promise starts.

## Until release

Harrow is built by [Zkeleton](https://zkeleton.com). The product page is at [zkeleton.com/harrow](https://www.zkeleton.com/harrow).
