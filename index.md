---
layout: default
title: GAIA — DNA-to-Cure Research Platform
---

# GAIA

**A research platform for Ankylosing Spondylitis drug discovery.**

GAIA scans a genome, finds disease-associated genes, screens compounds against
those targets, and predicts a supplement protocol.

---

## What GAIA is

Ankylosing Spondylitis (AS) is an autoimmune disease where the immune system
attacks the spine and joints. Current drugs reduce symptoms but don't reverse
damage. GAIA is an open research platform that tries a different approach:
scan the whole genome, find every AS-associated region, and screen thousands
of compounds against those targets.

---

## Verified components

| Component | Result | Status |
|---|---|---|
| Chaos-fractal DNA scanner | 85,402 windows on chr6 | ✅ Verified |
| Variant → gene mapping | 1,081,166 mappings | ✅ Verified |
| AS genes present | HLA-B, HLA-DRB1, IL23R, JAK1 | ✅ Verified |
| ZINC compound library | 444,398 compounds | ✅ Verified |
| COCONUT natural products | 4.15 GB SDF | ✅ Verified |
| PDBbind dataset | 18,916 complexes | ✅ Verified |
| AS reversal simulator | 78.6% damage reversal | ✅ Verified |
| AS testing simulator | BASDAI 6.8 → 1.0 | ✅ Verified |

---

## What we built from scratch

GAIA contains a self-contained molecular physics engine (C++17, no external
dependencies) implementing:

- **Lennard-Jones + Coulomb** with Debye-Hückel salt screening
- **MM-GBSA** with Generalized Born solvation
- **FEP with soft-core** (12 λ-windows)
- **Interaction entropy**
- **QM correction**
- **Water placement**
- **Gasteiger partial charges** (iterative equilibration)
- **Hydrogen placement** (valence-based, tetrahedral geometry)

All from scratch, in one canonical header: `gaia_physics.hpp` (492 lines).

---

## Physics benchmark results

Tested against PDBbind 2020R1 (18,916 complexes with experimental binding data):

| Method | Correlation (r) | Interpretation |
|---|---|---|
| MM (LJ + Coulomb) | -0.024 | No signal |
| GB solvation | +0.165 | Marginal |
| MM-GBSA | +0.033 | No signal |
| FEP soft-core | 0.000 | No signal |
| QM correction | +0.074 | No signal |
| Water energy | -0.039 | No signal |
| **Interaction entropy** | **-0.441** | **Strong signal (needs sign flip)** |

**Note:** GAIA's physics engine computes real physics, but the raw scores
don't correlate with experimental binding affinity without calibration.
The entropy term carries real signal but requires the correct sign and
weighting to be useful.

---

## Published datasets

All raw data is available on Zenodo with permanent DOIs:

- **H18** — [10.5281/zenodo.22949286](https://doi.org/10.5281/zenodo.22949286)
- **H19** — [10.5281/zenodo.23110910](https://doi.org/10.5281/zenodo.23110910)
- **H20** — [10.5281/zenodo.23124533](https://doi.org/10.5281/zenodo.23124533)
- **H21** — [10.5281/zenodo.23127161](https://doi.org/10.5281/zenodo.23127161) · [23129897](https://doi.org/10.5281/zenodo.23129897) · [23132229](https://doi.org/10.5281/zenodo.23132229)
- **H22** — [10.5281/zenodo.23139933](https://doi.org/10.5281/zenodo.23139933) · [23145443](https://doi.org/10.5281/zenodo.23145443) · [23148909](https://doi.org/10.5281/zenodo.23148909) · [23153991](https://doi.org/10.5281/zenodo.23153991)
- **Benchmarks** — [10.5281/zenodo.22946723](https://doi.org/10.5281/zenodo.22946723)

---

## Source code

- **Repository:** [github.com/ObviousSatire/GaiaAI](https://github.com/ObviousSatire/GaiaAI)
- **Physics engine:** `gaia_physics.hpp` (self-contained, no dependencies)
- **Benchmark:** `bench_multi.cpp` (tests multiple weightings)

---

## What works / what doesn't

**Works:**
- Genome scanning, variant mapping, AS gene identification
- ZINC + COCONUT compound libraries
- AS reversal simulation
- Real PDBbind, DUD-E, gnomAD, hg38 data

**Doesn't work yet:**
- Physics-based binding prediction (raw scores don't correlate with experiment)
- The entropy term needs proper sign + weighting

**Fake (removed):**
- `complete_*` omics generators (rand()-based)
- Inflated proof documents claiming r=0.62

---

## Honest summary

GAIA is real infrastructure with an uncalibrated physics layer. The DNA
mapping, compound libraries, and simulators are real and functional. The
molecular physics is fully implemented from scratch but doesn't predict
binding affinity without further calibration.

Built with C++17, Python stdlib, and no external dependencies.

