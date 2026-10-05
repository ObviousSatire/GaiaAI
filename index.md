---
layout: null
---
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GAIA — DNA-to-Cure Platform for Ankylosing Spondylitis</title>
<meta name="description" content="A computational platform for Ankylosing Spondylitis drug discovery: genome scanning, compound screening, and reversal protocol design.">
<link rel="stylesheet" href="assets/style.css">
</head>
<body>

<div class="hero">
    <div class="container">
        <h1>GAIA</h1>
        <p class="tagline">
            A DNA-to-cure platform for Ankylosing Spondylitis research.
            Genome scanning, compound discovery, and protocol design — end to end.
        </p>
        <div class="badges">
            <span class="badge"><strong>85,402</strong> chr6 windows scanned</span>
            <span class="badge"><strong>1.08M</strong> variant mappings</span>
            <span class="badge"><strong>444,398</strong> compounds screened</span>
            <span class="badge"><strong>10+</strong> published datasets</span>
        </div>
    </div>
</div>

<section>
    <div class="container">
        <h2>What GAIA does</h2>
        <p>
            GAIA takes a genome and produces a treatment protocol. It finds
            disease-associated regions, maps them to genes, screens thousands
            of compounds against those targets, and outputs a ranked protocol
            with predicted outcomes.
        </p>

        <div class="cards">
            <div class="card">
                <div class="metric">85,402</div>
                <div class="metric-sub">chr6 windows classified</div>
            </div>
            <div class="card">
                <div class="metric">1,081,166</div>
                <div class="metric-sub">variant→gene mappings</div>
            </div>
            <div class="card">
                <div class="metric">444,398</div>
                <div class="metric-sub">ZINC compounds</div>
            </div>
            <div class="card">
                <div class="metric">78.6%</div>
                <div class="metric-sub">damage reversal predicted</div>
            </div>
            <div class="card">
                <div class="metric">18,916</div>
                <div class="metric-sub">PDBbind complexes</div>
            </div>
            <div class="card">
                <div class="metric">4.15 GB</div>
                <div class="metric-sub">natural products (COCONUT)</div>
            </div>
        </div>
    </div>
</section>

<section>
    <div class="container">
        <h2>Core capabilities</h2>

        <div class="features">
            <div class="feature">
                <div class="icon">🧬</div>
                <h4>Chaos-fractal genome scanner</h4>
                <p>Classifies every window of a chromosome by fractal dimension and GC content. Correctly identifies the HLA-B region as coding-GC-rich.</p>
            </div>
            <div class="feature">
                <div class="icon">🔗</div>
                <h4>Variant-to-gene mapping</h4>
                <p>Over 1 million 1000G European variants mapped to Ensembl gene coordinates, filtered by allele frequency.</p>
            </div>
            <div class="feature">
                <div class="icon">💊</div>
                <h4>Compound library screening</h4>
                <p>444,398 ZINC compounds + 4.15 GB of COCONUT natural products, screened against AS targets.</p>
            </div>
            <div class="feature">
                <div class="icon">🔬</div>
                <h4>Molecular physics engine</h4>
                <p>Self-contained C++17 implementation: Lennard-Jones, Coulomb, Generalized Born, FEP, entropy, QM.</p>
            </div>
            <div class="feature">
                <div class="icon">📊</div>
                <h4>Protocol simulator</h4>
                <p>Multi-compound reversal protocols with predicted damage reversal, joint function restoration, and safety profiles.</p>
            </div>
            <div class="feature">
                <div class="icon">📦</div>
                <h4>Reproducible datasets</h4>
                <p>Every dataset published on Zenodo with permanent DOIs. Full pipeline reproducible from raw inputs.</p>
            </div>
        </div>
    </div>
</section>

<section>
    <div class="container">
        <h2>Physics engine</h2>
        <p>
            GAIA includes a self-contained molecular physics engine written from
            scratch in C++17 with no external dependencies. It implements the
            same methods used by established docking software, in a single
            canonical header.
        </p>

<pre><code>gaia_physics.hpp
├── Element data (10 elements, AMBER-derived)
├── Bond detection (covalent radii + distance)
├── Hydrogen placement (valence + tetrahedral)
├── Gasteiger partial charges (iterative)
├── Lennard-Jones + Coulomb (Debye-Hückel)
├── Generalized Born solvation
├── SASA (solvent accessible surface)
├── MM-GBSA (single trajectory)
├── FEP with soft-core (12 λ-windows)
├── Interaction entropy (quasi-harmonic)
├── QM correction (Hückel-like)
└── Water placement (grid scan)</code></pre>
    </div>
</section>

<section>
    <div class="container">
        <h2>Published datasets</h2>
        <p>
            All raw data is archived on Zenodo with permanent DOIs.
        </p>

        <table>
            <tr><th>Dataset</th><th>Size</th><th>DOI</th></tr>
            <tr><td>H18</td><td>25.7 GB</td><td><a href="https://doi.org/10.5281/zenodo.22949286">22949286</a></td></tr>
            <tr><td>H19</td><td>44.3 GB</td><td><a href="https://doi.org/10.5281/zenodo.23110910">23110910</a></td></tr>
            <tr><td>H20</td><td>45.1 GB</td><td><a href="https://doi.org/10.5281/zenodo.23124533">23124533</a></td></tr>
            <tr><td>H21</td><td>93.7 GB</td><td><a href="https://doi.org/10.5281/zenodo.23127161">23127161</a></td></tr>
            <tr><td>H22</td><td>128.7 GB</td><td><a href="https://doi.org/10.5281/zenodo.23139933">23139933</a></td></tr>
            <tr><td>Benchmarks</td><td>20 GB</td><td><a href="https://doi.org/10.5281/zenodo.22946723">22946723</a></td></tr>
        </table>
    </div>
</section>

<section>
    <div class="container">
        <h2>Reproducible from raw inputs</h2>
        <p>
            GAIA operates on publicly available biological data:
        </p>
        <ul style="color: var(--fg-dim); margin-left: 20px; line-height: 2;">
            <li>hg38 reference genome (3.1 GB)</li>
            <li>1000 Genomes Phase 3 EUR variants (946,650)</li>
            <li>Ensembl release 110 gene annotations (62,754 genes)</li>
            <li>gnomAD v4.0 population frequencies (66 GB chr1)</li>
            <li>BindingDB binding affinities (8.5 GB)</li>
            <li>PDBbind 2020R1 benchmark (18,916 complexes)</li>
            <li>DUD-E actives + decoys (102 targets)</li>
            <li>COCONUT natural products (4.15 GB)</li>
        </ul>
    </div>
</section>

<footer>
    <div class="container">
        <p>
            <a href="https://github.com/ObviousSatire/GaiaAI">Source on GitHub</a>
            &nbsp;·&nbsp;
            <a href="https://doi.org/10.5281/zenodo.22949286">Zenodo datasets</a>
        </p>
        <p style="margin-top: 16px; font-size: 0.8rem;">
            Built with C++17 and Python stdlib. No external dependencies.
        </p>
    </div>
</footer>

</body>
</html>
