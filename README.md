# GAIA

**A self-learning DNA-to-cure platform for disease research.**

Website: [obvioussatire.github.io/GaiaAI](https://obvioussatire.github.io/GaiaAI)

## Self-learning, two layers

**Layer 1 — Genome grammar.** Learns the structure of the genome from raw sequence and GENCODE labels. Discovers its own thresholds and features.

**Layer 2 — Function discovery.** Learns which variants cause which diseases, which compounds hit which proteins. Grows a graph automatically as data arrives.

The two layers connect: genome features feed the disease classifier; the disease classifier uses them to improve prediction.

## Capabilities

- Chaos-fractal genome scanner
- Variant-to-gene mapping (over 1 million variants)
- Self-learning disease graph
- Seven compound libraries (ZINC, COCONUT, ChEMBL, more)
- Nine-method molecular physics engine (self-contained C++17)
- Protocol simulator
- Link prediction classifier
- Reproducible datasets — 380+ GB on Zenodo

## Build

Pure C++17 and Python stdlib. No external dependencies.
