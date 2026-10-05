---
layout: null
---
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GAIA — DNA-to-Cure Platform for Ankylosing Spondylitis</title>
<meta name="description" content="A computational platform for Ankylosing Spondylitis drug discovery. Genome scanning, compound screening, reversal protocol design.">
<link rel="stylesheet" href="assets/style.css">
</head>
<body>

<div class="hero">
    <svg class="hero-bg" viewBox="0 0 1200 600" preserveAspectRatio="xMidYMid slice">
        <defs>
            <linearGradient id="helixGrad" x1="0%" y1="0%" x2="100%" y2="0%">
                <stop offset="0%" stop-color="#4ade80" stop-opacity="0.6"/>
                <stop offset="50%" stop-color="#60a5fa" stop-opacity="0.6"/>
                <stop offset="100%" stop-color="#a78bfa" stop-opacity="0.6"/>
            </linearGradient>
        </defs>
        <g transform="translate(600, 300)" opacity="0.4">
            <path d="M-500,0 Q-250,-150 0,0 T500,0" stroke="url(#helixGrad)" stroke-width="1.5" fill="none"/>
            <path d="M-500,0 Q-250,150 0,0 T500,0" stroke="url(#helixGrad)" stroke-width="1.5" fill="none"/>
            <path d="M-450,20 Q-250,-130 0,20 T450,20" stroke="url(#helixGrad)" stroke-width="1" fill="none" opacity="0.6"/>
            <path d="M-450,-20 Q-250,130 0,-20 T450,-20" stroke="url(#helixGrad)" stroke-width="1" fill="none" opacity="0.6"/>
            <path d="M-400,40 Q-250,-110 0,40 T400,40" stroke="url(#helixGrad)" stroke-width="0.8" fill="none" opacity="0.4"/>
            <path d="M-400,-40 Q-250,110 0,-40 T400,-40" stroke="url(#helixGrad)" stroke-width="0.8" fill="none" opacity="0.4"/>
        </g>
        <g opacity="0.3">
            <line x1="200" y1="290" x2="200" y2="310" stroke="#60a5fa" stroke-width="1"/>
            <line x1="300" y1="270" x2="300" y2="330" stroke="#a78bfa" stroke-width="1"/>
            <line x1="400" y1="250" x2="400" y2="350" stroke="#4ade80" stroke-width="1"/>
            <line x1="500" y1="240" x2="500" y2="360" stroke="#60a5fa" stroke-width="1"/>
            <line x1="700" y1="240" x2="700" y2="360" stroke="#60a5fa" stroke-width="1"/>
            <line x1="800" y1="250" x2="800" y2="350" stroke="#4ade80" stroke-width="1"/>
            <line x1="900" y1="270" x2="900" y2="330" stroke="#a78bfa" stroke-width="1"/>
            <line x1="1000" y1="290" x2="1000" y2="310" stroke="#60a5fa" stroke-width="1"/>
        </g>
    </svg>

    <div class="container hero-content">
        <svg class="hero-logo" width="80" height="80" viewBox="0 0 80 80">
            <defs>
                <linearGradient id="logoGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                    <stop offset="0%" stop-color="#4ade80"/>
                    <stop offset="100%" stop-color="#60a5fa"/>
                </linearGradient>
            </defs>
            <circle cx="40" cy="40" r="36" fill="none" stroke="url(#logoGrad)" stroke-width="2"/>
            <path d="M22,40 Q40,20 58,40 T22,40" fill="none" stroke="url(#logoGrad)" stroke-width="2"/>
            <path d="M22,40 Q40,60 58,40 T22,40" fill="none" stroke="url(#logoGrad)" stroke-width="2"/>
            <circle cx="40" cy="40" r="3" fill="#4ade80"/>
        </svg>

        <h1>GAIA</h1>
        <p class="tagline">
            A DNA-to-cure platform for <strong>Ankylosing Spondylitis</strong>.
            Scan a genome, find disease-associated genes, screen compounds against
            those targets, and design a treatment protocol — end to end.
        </p>

        <div class="hero-cta">
            <a href="#pipeline" class="btn btn-primary">See the pipeline →</a>
            <a href="https://github.com/ObviousSatire/GaiaAI" class="btn">View source</a>
        </div>

        <div class="stats">
            <div class="stat">
                <div class="num" data-count="85402">0</div>
                <div class="label">Chr6 windows</div>
            </div>
            <div class="stat">
                <div class="num" data-count="1081166" data-format="k">0</div>
                <div class="label">Variant mappings</div>
            </div>
            <div class="stat">
                <div class="num" data-count="444398">0</div>
                <div class="label">ZINC compounds</div>
            </div>
            <div class="stat">
                <div class="num" data-count="18916">0</div>
                <div class="label">PDBbind complexes</div>
            </div>
        </div>
    </div>
</div>

<section>
    <div class="container-narrow">
        <h2>Why <span class="accent">Ankylosing Spondylitis</span></h2>
        <p class="lead">
            AS is an autoimmune disease where the immune system attacks the
            spine and joints, eventually fusing vertebrae. Current drugs reduce
            symptoms but don't reverse damage. GAIA starts with the whole genome
            instead of a hypothesis.
        </p>
        <div class="context-box">
            <h3>Disease burden</h3>
            <p>
                AS affects roughly 0.5% of the population, with strong HLA-B27
                association. Diagnosis typically happens years after symptom
                onset. Once vertebrae fuse (ankylosis), damage is permanent.
                The goal isn't just remission — it's stopping damage before it
                happens.
            </p>
        </div>
    </div>
</section>

<section id="pipeline">
    <div class="container">
        <h2>The <span class="accent">pipeline</span></h2>
        <p class="lead">Five stages from raw genome to treatment protocol.</p>

        <div class="pipeline">
            <div class="stage">
                <div class="stage-num">STAGE 01</div>
                <svg width="40" height="40" viewBox="0 0 40 40">
                    <circle cx="20" cy="20" r="16" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <path d="M8,20 Q20,10 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <path d="M8,20 Q20,30 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                </svg>
                <h3>Scan genome</h3>
                <p>Chaos-fractal analysis classifies every window by fractal dimension and GC content.</p>
            </div>
            <div class="stage">
                <div class="stage-num">STAGE 02</div>
                <svg width="40" height="40" viewBox="0 0 40 40">
                    <circle cx="10" cy="20" r="4" fill="#60a5fa"/>
                    <circle cx="30" cy="20" r="4" fill="#60a5fa"/>
                    <line x1="14" y1="20" x2="26" y2="20" stroke="#60a5fa" stroke-width="1.5"/>
                    <line x1="10" y1="16" x2="10" y2="10" stroke="#60a5fa" stroke-width="1.5"/>
                    <line x1="30" y1="24" x2="30" y2="30" stroke="#60a5fa" stroke-width="1.5"/>
                </svg>
                <h3>Map variants</h3>
                <p>1000 Genomes European variants mapped to Ensembl gene coordinates.</p>
            </div>
            <div class="stage">
                <div class="stage-num">STAGE 03</div>
                <svg width="40" height="40" viewBox="0 0 40 40">
                    <rect x="8" y="12" width="24" height="16" rx="3" fill="none" stroke="#a78bfa" stroke-width="1.5"/>
                    <line x1="14" y1="12" x2="14" y2="8" stroke="#a78bfa" stroke-width="1.5"/>
                    <line x1="26" y1="12" x2="26" y2="8" stroke="#a78bfa" stroke-width="1.5"/>
                    <circle cx="20" cy="20" r="3" fill="#a78bfa"/>
                </svg>
                <h3>Screen compounds</h3>
                <p>444,398 ZINC compounds and 4.15 GB of COCONUT natural products.</p>
            </div>
            <div class="stage">
                <div class="stage-num">STAGE 04</div>
                <svg width="40" height="40" viewBox="0 0 40 40">
                    <path d="M20,4 L36,14 L36,26 L20,36 L4,26 L4,14 Z" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="20" cy="20" r="4" fill="#4ade80"/>
                </svg>
                <h3>Score binding</h3>
                <p>Molecular physics: Lennard-Jones, Coulomb, GB solvation, FEP, entropy, QM.</p>
            </div>
            <div class="stage">
                <div class="stage-num">STAGE 05</div>
                <svg width="40" height="40" viewBox="0 0 40 40">
                    <path d="M8,20 L16,28 L32,12" fill="none" stroke="#60a5fa" stroke-width="2.5" stroke-linecap="round"/>
                </svg>
                <h3>Design protocol</h3>
                <p>Ranked multi-compound reversal with damage prediction and safety profile.</p>
            </div>
        </div>
    </div>
</section>

<section>
    <div class="container">
        <h2>What GAIA <span class="accent">delivers</span></h2>
        <p class="lead">Six integrated subsystems, working from raw genome to protocol.</p>

        <div class="features">
            <div class="feature">
                <svg width="36" height="36" viewBox="0 0 36 36">
                    <path d="M18,4 Q28,14 18,24 Q8,14 18,4 Z" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <path d="M18,12 Q24,18 18,24 Q12,18 18,12 Z" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <line x1="18" y1="24" x2="18" y2="32" stroke="#4ade80" stroke-width="1.5"/>
                </svg>
                <h3>Chaos-fractal scanner</h3>
                <p>Classifies chromosome windows by fractal dimension, Hurst exponent, and GC content. Identifies coding regions and conserved patterns across 170M bp in about 10 minutes.</p>
            </div>
            <div class="feature">
                <svg width="36" height="36" viewBox="0 0 36 36">
                    <circle cx="9" cy="18" r="3" fill="#60a5fa"/>
                    <circle cx="18" cy="9" r="3" fill="#60a5fa"/>
                    <circle cx="27" cy="18" r="3" fill="#60a5fa"/>
                    <circle cx="18" cy="27" r="3" fill="#60a5fa"/>
                    <line x1="9" y1="18" x2="18" y2="9" stroke="#60a5fa" stroke-width="1"/>
                    <line x1="18" y1="9" x2="27" y2="18" stroke="#60a5fa" stroke-width="1"/>
                    <line x1="27" y1="18" x2="18" y2="27" stroke="#60a5fa" stroke-width="1"/>
                    <line x1="18" y1="27" x2="9" y2="18" stroke="#60a5fa" stroke-width="1"/>
                </svg>
                <h3>Variant-to-gene mapping</h3>
                <p>Over one million European variants mapped to gene coordinates. AS-relevant genes identified with allele frequencies: HLA-B, HLA-DRB1, IL23R, JAK1, and more.</p>
            </div>
            <div class="feature">
                <svg width="36" height="36" viewBox="0 0 36 36">
                    <rect x="4" y="14" width="8" height="8" rx="1" fill="#a78bfa"/>
                    <rect x="14" y="14" width="8" height="8" rx="1" fill="#a78bfa" opacity="0.7"/>
                    <rect x="24" y="14" width="8" height="8" rx="1" fill="#a78bfa" opacity="0.5"/>
                    <line x1="12" y1="18" x2="14" y2="18" stroke="#a78bfa" stroke-width="1"/>
                    <line x1="22" y1="18" x2="24" y2="18" stroke="#a78bfa" stroke-width="1"/>
                </svg>
                <h3>Compound screening</h3>
                <p>ZINC 3D compound library plus COCONUT natural products, screened against AS targets. Real docking parameters, real scores, real rankings.</p>
            </div>
            <div class="feature">
                <svg width="36" height="36" viewBox="0 0 36 36">
                    <circle cx="18" cy="18" r="12" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="18" cy="18" r="6" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="18" cy="18" r="2" fill="#4ade80"/>
                    <line x1="18" y1="6" x2="18" y2="0" stroke="#4ade80" stroke-width="1.5"/>
                    <line x1="30" y1="18" x2="36" y2="18" stroke="#4ade80" stroke-width="1.5"/>
                </svg>
                <h3>Molecular physics</h3>
                <p>Self-contained C++17 engine. Lennard-Jones, Coulomb, Generalized Born, FEP, entropy, QM. No external dependencies.</p>
            </div>
            <div class="feature">
                <svg width="36" height="36" viewBox="0 0 36 36">
                    <path d="M6,28 L6,20 L12,20 L12,14 L18,14 L18,22 L24,22 L24,10 L30,10" fill="none" stroke="#60a5fa" stroke-width="2" stroke-linejoin="round"/>
                    <circle cx="6" cy="28" r="2" fill="#60a5fa"/>
                    <circle cx="30" cy="10" r="2" fill="#60a5fa"/>
                </svg>
                <h3>Protocol simulator</h3>
                <p>Multi-compound reversal protocols with predicted damage reversal, joint function restoration, disease risk, and safety profiles at 30, 90, 180, and 365 days.</p>
            </div>
            <div class="feature">
                <svg width="36" height="36" viewBox="0 0 36 36">
                    <ellipse cx="18" cy="12" rx="12" ry="4" fill="none" stroke="#a78bfa" stroke-width="1.5"/>
                    <path d="M6,12 L6,24 Q6,28 18,28 Q30,28 30,24 L30,12" fill="none" stroke="#a78bfa" stroke-width="1.5"/>
                    <path d="M6,18 Q6,22 18,22 Q30,22 30,18" fill="none" stroke="#a78bfa" stroke-width="1.5"/>
                </svg>
                <h3>Reproducible datasets</h3>
                <p>Every dataset published on Zenodo with permanent DOIs. Over 380 GB of raw inputs, intermediate results, and benchmarks — fully reproducible.</p>
            </div>
        </div>
    </div>
</section>

<section id="physics">
    <div class="container">
        <h2>Physics <span class="accent">engine</span></h2>
        <p class="lead">
            A self-contained molecular physics engine, written from scratch in
            C++17. Nine methods in one canonical header — no external libraries,
            no toolkits, no dependencies.
        </p>

        <div class="physics-grid">
            <div class="physics-item">
                <svg width="24" height="24" viewBox="0 0 24 24"><circle cx="12" cy="12" r="3" fill="#4ade80"/><circle cx="4" cy="4" r="2" fill="#4ade80" opacity="0.5"/><circle cx="20" cy="4" r="2" fill="#4ade80" opacity="0.5"/><circle cx="4" cy="20" r="2" fill="#4ade80" opacity="0.5"/><circle cx="20" cy="20" r="2" fill="#4ade80" opacity="0.5"/></svg>
                <div><div class="name">Lennard-Jones + Coulomb</div><div class="detail">with Debye-Hückel salt screening</div></div>
            </div>
            <div class="physics-item">
                <svg width="24" height="24" viewBox="0 0 24 24"><ellipse cx="12" cy="12" rx="10" ry="6" fill="none" stroke="#60a5fa" stroke-width="1.5"/><circle cx="12" cy="12" r="3" fill="#60a5fa"/></svg>
                <div><div class="name">Generalized Born</div><div class="detail">implicit solvation (HCT model)</div></div>
            </div>
            <div class="physics-item">
                <svg width="24" height="24" viewBox="0 0 24 24"><path d="M2,12 Q12,4 22,12 Q12,20 2,12" fill="none" stroke="#a78bfa" stroke-width="1.5"/><circle cx="12" cy="12" r="2" fill="#a78bfa"/></svg>
                <div><div class="name">MM-GBSA</div><div class="detail">single-trajectory binding energy</div></div>
            </div>
            <div class="physics-item">
                <svg width="24" height="24" viewBox="0 0 24 24"><path d="M2,18 L6,12 L10,16 L14,8 L18,14 L22,6" fill="none" stroke="#4ade80" stroke-width="1.5"/></svg>
                <div><div class="name">FEP with soft-core</div><div class="detail">12 lambda-windows, alchemical</div></div>
            </div>
            <div class="physics-item">
                <svg width="24" height="24" viewBox="0 0 24 24"><path d="M12,4 Q16,12 12,20 Q8,12 12,4" fill="none" stroke="#60a5fa" stroke-width="1.5"/><path d="M4,12 Q12,8 20,12 Q12,16 4,12" fill="none" stroke="#60a5fa" stroke-width="1.5"/></svg>
                <div><div class="name">Interaction entropy</div><div class="detail">quasi-harmonic approximation</div></div>
            </div>
            <div class="physics-item">
                <svg width="24" height="24" viewBox="0 0 24 24"><circle cx="12" cy="12" r="4" fill="none" stroke="#a78bfa" stroke-width="1.5"/><ellipse cx="12" cy="12" rx="10" ry="4" fill="none" stroke="#a78bfa" stroke-width="1"/><ellipse cx="12" cy="12" rx="4" ry="10" fill="none" stroke="#a78bfa" stroke-width="1"/></svg>
                <div><div class="name">QM correction</div><div class="detail">semi-empirical orbital terms</div></div>
            </div>
            <div class="physics-item">
                <svg width="24" height="24" viewBox="0 0 24 24"><circle cx="12" cy="14" r="4" fill="none" stroke="#4ade80" stroke-width="1.5"/><path d="M8,10 Q12,4 16,10" fill="none" stroke="#4ade80" stroke-width="1.5"/></svg>
                <div><div class="name">Water placement</div><div class="detail">grid-based pocket scan</div></div>
            </div>
            <div class="physics-item">
                <svg width="24" height="24" viewBox="0 0 24 24"><path d="M4,12 L8,12 L10,6 L14,18 L16,12 L20,12" fill="none" stroke="#60a5fa" stroke-width="1.5"/></svg>
                <div><div class="name">Gasteiger charges</div><div class="detail">iterative charge equilibration</div></div>
            </div>
            <div class="physics-item">
                <svg width="24" height="24" viewBox="0 0 24 24"><circle cx="7" cy="12" r="3" fill="none" stroke="#a78bfa" stroke-width="1.5"/><circle cx="17" cy="12" r="3" fill="none" stroke="#a78bfa" stroke-width="1.5"/><line x1="10" y1="12" x2="14" y2="12" stroke="#a78bfa" stroke-width="1.5"/></svg>
                <div><div class="name">Hydrogen placement</div><div class="detail">valence-based, tetrahedral</div></div>
            </div>
        </div>

        <div class="code-block">
<span class="comment">// gaia_physics.hpp — 492 lines, zero dependencies</span>
<span class="key">namespace</span> gaia {
    <span class="comment">// Element data, bond detection, H placement, Gasteiger charges</span>
    <span class="comment">// LJ + Coulomb + Debye-Hückel, GB solvation, SASA</span>
    <span class="comment">// MM-GBSA, FEP soft-core, entropy, QM, water</span>
    <span class="key">struct</span> ScoreBreakdown { ... };
    <span class="key">inline</span> ScoreBreakdown score(<span class="key">const</span> vector&lt;Atom&gt;&amp; lig, <span class="key">const</span> vector&lt;Atom&gt;&amp; rec);
}
        </div>
    </div>
</section>

<section>
    <div class="container">
        <h2>Published <span class="accent">datasets</span></h2>
        <p class="lead">
            All raw data archived on Zenodo with permanent DOIs. Fully
            reproducible from public sources.
        </p>

        <table class="data-table">
            <tr>
                <th>Dataset</th>
                <th>Size</th>
                <th>Files</th>
                <th>DOI</th>
            </tr>
            <tr>
                <td>H18 — ZINC shards</td>
                <td>25.7 GB</td>
                <td>53</td>
                <td><a href="https://doi.org/10.5281/zenodo.22949286">22949286</a></td>
            </tr>
            <tr>
                <td>H19 — compound library</td>
                <td>44.3 GB</td>
                <td>264,123</td>
                <td><a href="https://doi.org/10.5281/zenodo.23110910">23110910</a></td>
            </tr>
            <tr>
                <td>H20 — compound library</td>
                <td>45.1 GB</td>
                <td>321,494</td>
                <td><a href="https://doi.org/10.5281/zenodo.23124533">23124533</a></td>
            </tr>
            <tr>
                <td>H21 — compound library</td>
                <td>93.7 GB</td>
                <td>374,993</td>
                <td><a href="https://doi.org/10.5281/zenodo.23127161">23127161</a></td>
            </tr>
            <tr>
                <td>H22 — compound library</td>
                <td>128.7 GB</td>
                <td>428,028</td>
                <td><a href="https://doi.org/10.5281/zenodo.23139933">23139933</a></td>
            </tr>
            <tr>
                <td>Benchmarks — PDBbind, DUD-E, FEP+</td>
                <td>20 GB</td>
                <td>77,776</td>
                <td><a href="https://doi.org/10.5281/zenodo.22946723">22946723</a></td>
            </tr>
        </table>
    </div>
</section>

<section>
    <div class="container">
        <h2>Built on <span class="accent">public data</span></h2>
        <p class="lead">
            Every stage of GAIA runs on publicly available biological data.
        </p>

        <div class="features">
            <div class="feature">
                <h3>hg38 reference genome</h3>
                <p>3.1 GB human reference. Chaos-fractal analysis of chromosome 6 identifies HLA-B region structure.</p>
            </div>
            <div class="feature">
                <h3>1000 Genomes EUR</h3>
                <p>946,650 variants from European populations. Allele frequencies mapped to gene coordinates.</p>
            </div>
            <div class="feature">
                <h3>Ensembl 110</h3>
                <p>62,754 gene annotations with GRCh38 coordinates. Authoritative gene models.</p>
            </div>
            <div class="feature">
                <h3>gnomAD v4.0</h3>
                <p>66 GB population variant frequencies. Real human genetic diversity at scale.</p>
            </div>
            <div class="feature">
                <h3>PDBbind 2020R1</h3>
                <p>18,916 protein-ligand complexes with experimental binding data. Standard benchmark for physics validation.</p>
            </div>
            <div class="feature">
                <h3>ZINC + COCONUT</h3>
                <p>444,398 purchasable compounds plus 4.15 GB of natural products. The full screening universe.</p>
            </div>
        </div>
    </div>
</section>

<footer>
    <div class="container">
        <div class="footer-links">
            <a href="https://github.com/ObviousSatire/GaiaAI">Source on GitHub</a>
            <a href="https://doi.org/10.5281/zenodo.22949286">Zenodo datasets</a>
            <a href="#physics">Physics engine</a>
        </div>
        <p>Built with C++17 and Python stdlib. No external dependencies.</p>
    </div>
</footer>

<script>
const counters = document.querySelectorAll('.num[data-count]');
const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
        if (!entry.isIntersecting) return;
        const el = entry.target;
        const target = parseInt(el.dataset.count);
        const fmt = el.dataset.format;
        const duration = 1500;
        const start = performance.now();
        function update(now) {
            const t = Math.min(1, (now - start) / duration);
            const ease = 1 - Math.pow(1 - t, 3);
            const val = Math.floor(target * ease);
            if (fmt === 'k' && val >= 1000) {
                el.textContent = (val / 1000).toFixed(2).replace(/\.00$/, '') + 'M';
            } else {
                el.textContent = val.toLocaleString();
            }
            if (t < 1) requestAnimationFrame(update);
        }
        requestAnimationFrame(update);
        observer.unobserve(el);
    });
}, { threshold: 0.3 });
counters.forEach(c => observer.observe(c));
</script>

</body>
</html>
