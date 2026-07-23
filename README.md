# Harrow

**Open-source release in preparation.** This repository is the reserved public home for the Harrow engine. The code lands here when our first deployment is live; this page exists so the commitment is public before the release is.

## What Harrow is

Harrow is a deterministic screening engine for Medicare Advantage risk-adjustment data. It implements the structural logic of HHS-OIG Toolkit A-07-23-01213 — the published federal methodology for identifying high-risk diagnosis-code patterns — as verifiable code rather than a black box:

- Toolkit-cited code lists with hashed provenance, traceable line-by-line to the OIG source documents
- A stage-matrix executor that evaluates each screening stage exactly as the toolkit defines it, including the places where the toolkit's narrative and its printed SQL disagree (both interpretations are carried, documented as named deviations)
- An independently implemented reference oracle used to prove stage-level parity with the engine, with mutation-tested checks

## Why open source

The people who evaluate a screening tool — compliance teams, special investigation units, risk-adjustment analysts — should be able to read exactly what the screen does. Auditability is not a feature of this product; it is the product. Publishing the engine is the strongest form of that claim.

## What stays commercial

Harrow is built by [Zkeleton](https://zkeleton.com). The open-source engine is the reference implementation of the public OIG methodology. Current-model-year screen packs, hosted review surfaces, in-environment deployment, signing, and support are part of the commercial Zkeleton service.

## Until release

The product walkthrough is live at [zkeleton.com/harrow](https://zkeleton.com/harrow).
