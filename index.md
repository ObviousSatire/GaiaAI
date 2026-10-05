---
layout: null
---
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GAIA — DNA-to-Cure Platform</title>
<meta name="description" content="A computational platform for disease research. Genome scanning, compound screening, reversal protocol design.">
<link rel="stylesheet" href="assets/style.css">
</head>
<body>

<div class="hero">
    <svg class="hero-bg" viewBox="0 0 1600 700" preserveAspectRatio="xMidYMid slice">
        <defs>
            <linearGradient id="helixGrad" x1="0%" y1="0%" x2="100%" y2="0%">
                <stop offset="0%" stop-color="#4ade80" stop-opacity="0.7"/>
                <stop offset="50%" stop-color="#60a5fa" stop-opacity="0.7"/>
                <stop offset="100%" stop-color="#a78bfa" stop-opacity="0.7"/>
            </linearGradient>
        </defs>
        <g class="helix-path" transform="translate(800, 350)">
            <path d="M-800,0 Q-400,-180 0,0 T800,0" stroke="url(#helixGrad)" stroke-width="1.8" fill="none"/>
            <path d="M-800,0 Q-400,180 0,0 T800,0" stroke="url(#helixGrad)" stroke-width="1.8" fill="none"/>
            <path d="M-700,30 Q-400,-150 0,30 T700,30" stroke="url(#helixGrad)" stroke-width="1" fill="none" opacity="0.6"/>
            <path d="M-700,-30 Q-400,150 0,-30 T700,-30" stroke="url(#helixGrad)" stroke-width="1" fill="none" opacity="0.6"/>
        </g>
        <g class="float-dot" opacity="0.6">
            <circle cx="200" cy="150" r="2" fill="#4ade80"/>
            <circle cx="400" cy="550" r="2" fill="#60a5fa"/>
            <circle cx="1200" cy="200" r="2" fill="#a78bfa"/>
            <circle cx="1400" cy="500" r="2" fill="#4ade80"/>
            <circle cx="800" cy="120" r="2" fill="#60a5fa"/>
            <circle cx="300" cy="400" r="2" fill="#a78bfa"/>
            <circle cx="1300" cy="380" r="2" fill="#4ade80"/>
            <circle cx="600" cy="600" r="2" fill="#60a5fa"/>
            <circle cx="1000" cy="580" r="2" fill="#a78bfa"/>
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
            A DNA-to-cure platform. Scan a genome, find disease-associated
            genes, screen compounds against those targets, and design a
            treatment protocol — <strong>end to end</strong>.
        </p>

        <div class="hero-cta">
            <a href="#pipeline" class="btn btn-primary">Explore the pipeline →</a>
            <a href="https://github.com/ObviousSatire/GaiaAI" class="btn">View source</a>
        </div>

        <div class="stats">
            <div class="stat">
                <div class="num" data-count="1081166" data-format="k">0</div>
                <div class="label">Variant mappings</div>
            </div>
            <div class="stat">
                <div class="num" data-count="7" data-format="plus">0</div>
                <div class="label">Compound libraries</div>
            </div>
            <div class="stat">
                <div class="num" data-count="9" data-format="plus">0</div>
                <div class="label">Physics methods</div>
            </div>
            <div class="stat">
                <div class="num" data-count="380" data-format="gb">0</div>
                <div class="label">Data published</div>
            </div>
        </div>
    </div>
</div>

<section>
    <div class="container-narrow">
        <h2>A platform for <span class="accent">complex disease</span></h2>
        <p class="lead">
            Most drug discovery starts with a hypothesis and tests it. GAIA
            starts with the full genome — every variant, every gene, every
            pathway — and works backward to find what could help.
        </p>
        <div class="context-box">
            <h3>Designed to generalize</h3>
            <p>
                The pipeline isn't tied to one disease. Genome scanning,
                variant mapping, compound screening, and protocol simulation
                are all disease-agnostic. The first deployment is for an
                autoimmune condition, but the same architecture applies to
                inflammatory, neurodegenerative, and metabolic diseases.
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
                <p>Chaos-fractal analysis classifies every window by fractal dimension, Hurst exponent, and GC content — genome-wide.</p>
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
                <p>Over 1 million population variants mapped to gene coordinates, with allele frequencies and functional annotation.</p>
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
                <p>Seven compound libraries — including hundreds of thousands of purchasable molecules and natural products.</p>
            </div>
            <div class="stage">
                <div class="stage-num">STAGE 04</div>
                <svg width="40" height="40" viewBox="0 0 40 40">
                    <path d="M20,4 L36,14 L36,26 L20,36 L4,26 L4,14 Z" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="20" cy="20" r="4" fill="#4ade80"/>
                </svg>
                <h3>Score binding</h3>
                <p>Nine molecular physics methods, from Lennard-Jones to quantum corrections — a self-contained C++17 engine.</p>
            </div>
            <div class="stage">
                <div class="stage-num">STAGE 05</div>
                <svg width="40" height="40" viewBox="0 0 40 40">
                    <path d="M8,20 L16,28 L32,12" fill="none" stroke="#60a5fa" stroke-width="2.5" stroke-linecap="round"/>
                </svg>
                <h3>Design protocol</h3>
                <p>Ranked multi-compound protocol with predicted outcomes at 30, 90, 180, and 365 days.</p>
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
                <p>Classifies chromosome windows by fractal dimension and Hurst exponent. Identifies coding regions, conserved patterns, and structural signals across whole genomes.</p>
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
                <p>Over 1 million population variants mapped to gene coordinates. Allele frequencies, functional context, and gene-level aggregation at scale.</p>
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
                <p>Seven compound libraries covering purchasable small molecules, natural products, and known drugs. Real docking parameters, real scores, real rankings.</p>
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
                <p>A self-contained C++17 engine — nine physics methods, no external dependencies, no toolkits. Everything from Lennard-Jones to quantum corrections in one header.</p>
            </div>
            <div class="feature">
                <svg width="36" height="36" viewBox="0 0 36 36">
                    <path d="M6,28 L6,20 L12,20 L12,14 L18,14 L18,22 L24,22 L24,10 L30,10" fill="none" stroke="#60a5fa" stroke-width="2" stroke-linejoin="round"/>
                    <circle cx="6" cy="28" r="2" fill="#60a5fa"/>
                    <circle cx="30" cy="10" r="2" fill="#60a5fa"/>
                </svg>
                <h3>Protocol simulator</h3>
                <p>Multi-compound protocol simulation with predicted outcomes across time — damage reversal, function restoration, risk profiles, and safety margins.</p>
            </div>
            <div class="feature">
                <svg width="36" height="36" viewBox="0 0 36 36">
                    <ellipse cx="18" cy="12" rx="12" ry="4" fill="none" stroke="#a78bfa" stroke-width="1.5"/>
                    <path d="M6,12 L6,24 Q6,28 18,28 Q30,28 30,24 L30,12" fill="none" stroke="#a78bfa" stroke-width="1.5"/>
                    <path d="M6,18 Q6,22 18,22 Q30,22 30,18" fill="none" stroke="#a78bfa" stroke-width="1.5"/>
                </svg>
                <h3>Reproducible datasets</h3>
                <p>Every dataset archived on Zenodo with permanent DOIs. Over 380 GB of raw inputs, intermediate results, and benchmarks — reproducible from public sources.</p>
            </div>
        </div>
    </div>
</section>

<section id="physics">
    <div class="container">
        <h2>Physics <span class="accent">engine</span></h2>
        <p class="lead">
            Nine molecular physics methods, written from scratch in C++17.
            One canonical header. Zero external dependencies.
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
<span class="comment">// gaia_physics.hpp — one header, zero dependencies</span>
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
            Every stage archived on Zenodo with permanent DOIs. Reproducible
            from public sources.
        </p>

        <table class="data-table">
            <tr>
                <th>Dataset</th>
                <th>Size</th>
                <th>Contents</th>
                <th>DOI</th>
            </tr>
            <tr>
                <td>Compound library I</td>
                <td>25.7 GB</td>
                <td>ZINC shards</td>
                <td><a href="https://doi.org/10.5281/zenodo.22949286">22949286</a></td>
            </tr>
            <tr>
                <td>Compound library II</td>
                <td>44.3 GB</td>
                <td>ZINC compound set</td>
                <td><a href="https://doi.org/10.5281/zenodo.23110910">23110910</a></td>
            </tr>
            <tr>
                <td>Compound library III</td>
                <td>45.1 GB</td>
                <td>ZINC compound set</td>
                <td><a href="https://doi.org/10.5281/zenodo.23124533">23124533</a></td>
            </tr>
            <tr>
                <td>Compound library IV</td>
                <td>93.7 GB</td>
                <td>ZINC compound set</td>
                <td><a href="https://doi.org/10.5281/zenodo.23127161">23127161</a></td>
            </tr>
            <tr>
                <td>Compound library V</td>
                <td>128.7 GB</td>
                <td>ZINC compound set</td>
                <td><a href="https://doi.org/10.5281/zenodo.23139933">23139933</a></td>
            </tr>
            <tr>
                <td>Benchmarks</td>
                <td>20 GB</td>
                <td>PDBbind, DUD-E, FEP+</td>
                <td><a href="https://doi.org/10.5281/zenodo.22946723">22946723</a></td>
            </tr>
        </table>
    </div>
</section>

<section>
    <div class="container">
        <h2>Built on <span class="accent">public data</span></h2>
        <p class="lead">
            Every stage of GAIA runs on publicly available biological data —
            no proprietary datasets, no hidden inputs.
        </p>

        <div class="features">
            <div class="feature">
                <h3>Reference genomes</h3>
                <p>Human reference assemblies, gene annotations, and population cohorts. The chaos-fractal scanner and variant mapper both work on standard formats.</p>
            </div>
            <div class="feature">
                <h3>Population genetics</h3>
                <p>Over a million variants from public population studies. Allele frequencies mapped to gene coordinates with functional context.</p>
            </div>
            <div class="feature">
                <h3>Gene annotations</h3>
                <p>Tens of thousands of curated gene models with GRCh38 coordinates. Authoritative sources for gene boundaries and transcripts.</p>
            </div>
            <div class="feature">
                <h3>Population frequencies</h3>
                <p>Dozens of gigabytes of population-scale variant frequencies. Real human genetic diversity used as the base layer.</p>
            </div>
            <div class="feature">
                <h3>Binding benchmarks</h3>
                <p>Tens of thousands of protein-ligand complexes with experimental binding data. The standard benchmark for scoring function validation.</p>
            </div>
            <div class="feature">
                <h3>Compound libraries</h3>
                <p>Hundreds of thousands of purchasable compounds plus gigabytes of natural products. The full screening universe in standard formats.</p>
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
// Animated counters
const counters = document.querySelectorAll('.num[data-count]');
const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
        if (!entry.isIntersecting) return;
        const el = entry.target;
        const target = parseInt(el.dataset.count);
        const fmt = el.dataset.format;
        const duration = 1800;
        const start = performance.now();
        function update(now) {
            const t = Math.min(1, (now - start) / duration);
            const ease = 1 - Math.pow(1 - t, 3);
            const val = Math.floor(target * ease);
            if (fmt === 'k' && val >= 1000) {
                el.textContent = (val / 1000).toFixed(2).replace(/\.00$/, '') + 'M';
            } else if (fmt === 'plus') {
                el.textContent = val + '+';
            } else if (fmt === 'gb') {
                el.textContent = val + ' GB';
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

// Section fade-in on scroll
const sections = document.querySelectorAll('section');
const sectionObserver = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.classList.add('visible');
            sectionObserver.unobserve(entry.target);
        }
    });
}, { threshold: 0.1 });
sections.forEach(s => sectionObserver.observe(s));

// Parallax on hero background
const heroBg = document.querySelector('.hero-bg');
if (heroBg) {
    window.addEventListener('scroll', () => {
        const y = window.scrollY;
        if (y < window.innerHeight) {
            heroBg.style.transform = `translateY(${y * 0.3}px)`;
        }
    });
}
</script>

</body>
</html>
