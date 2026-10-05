---
layout: null
---
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GAIA — Self-Learning DNA-to-Cure Platform</title>
<meta name="description" content="A self-learning platform for disease research: genome scanning, variant mapping, compound discovery, and protocol design.">
<link rel="stylesheet" href="assets/style.css">
</head>
<body>

<div class="hero">
    <svg class="hero-bg" viewBox="0 0 1800 800" preserveAspectRatio="xMidYMid slice">
        <defs>
            <linearGradient id="helixGrad" x1="0%" y1="0%" x2="100%" y2="0%">
                <stop offset="0%" stop-color="#4ade80" stop-opacity="0.8"/>
                <stop offset="33%" stop-color="#60a5fa" stop-opacity="0.8"/>
                <stop offset="66%" stop-color="#a78bfa" stop-opacity="0.8"/>
                <stop offset="100%" stop-color="#f472b6" stop-opacity="0.8"/>
            </linearGradient>
        </defs>
        <g class="helix-path" transform="translate(900, 400)">
            <path d="M-1000,0 Q-500,-200 0,0 T1000,0" stroke="url(#helixGrad)" stroke-width="2" fill="none"/>
            <path d="M-1000,0 Q-500,200 0,0 T1000,0" stroke="url(#helixGrad)" stroke-width="2" fill="none"/>
            <path d="M-900,40 Q-500,-170 0,40 T900,40" stroke="url(#helixGrad)" stroke-width="1.2" fill="none" opacity="0.6"/>
            <path d="M-900,-40 Q-500,170 0,-40 T900,-40" stroke="url(#helixGrad)" stroke-width="1.2" fill="none" opacity="0.6"/>
            <path d="M-800,80 Q-500,-140 0,80 T800,80" stroke="url(#helixGrad)" stroke-width="0.8" fill="none" opacity="0.4"/>
            <path d="M-800,-80 Q-500,140 0,-80 T800,-80" stroke="url(#helixGrad)" stroke-width="0.8" fill="none" opacity="0.4"/>
        </g>
        <g>
            <circle class="particle" cx="180" cy="140" r="2.5" fill="#4ade80"/>
            <circle class="particle" cx="420" cy="620" r="2.5" fill="#60a5fa"/>
            <circle class="particle" cx="1380" cy="180" r="2.5" fill="#a78bfa"/>
            <circle class="particle" cx="1620" cy="540" r="2.5" fill="#f472b6"/>
            <circle class="particle" cx="900" cy="100" r="2.5" fill="#60a5fa"/>
            <circle class="particle" cx="260" cy="480" r="2.5" fill="#a78bfa"/>
            <circle class="particle" cx="1500" cy="400" r="2.5" fill="#4ade80"/>
            <circle class="particle" cx="700" cy="700" r="2.5" fill="#60a5fa"/>
            <circle class="particle" cx="1100" cy="650" r="2.5" fill="#a78bfa"/>
            <circle class="particle" cx="600" cy="260" r="2.5" fill="#f472b6"/>
            <circle class="particle" cx="1200" cy="320" r="2.5" fill="#4ade80"/>
            <circle class="particle" cx="340" cy="340" r="2.5" fill="#60a5fa"/>
        </g>
    </svg>

    <div class="container hero-content">
        <svg class="hero-logo" width="84" height="84" viewBox="0 0 80 80">
            <defs>
                <linearGradient id="logoGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                    <stop offset="0%" stop-color="#4ade80"/>
                    <stop offset="33%" stop-color="#60a5fa"/>
                    <stop offset="66%" stop-color="#a78bfa"/>
                    <stop offset="100%" stop-color="#f472b6"/>
                </linearGradient>
            </defs>
            <circle class="ring" cx="40" cy="40" r="36" fill="none" stroke="url(#logoGrad)" stroke-width="2"/>
            <path d="M22,40 Q40,20 58,40 T22,40" fill="none" stroke="url(#logoGrad)" stroke-width="2"/>
            <path d="M22,40 Q40,60 58,40 T22,40" fill="none" stroke="url(#logoGrad)" stroke-width="2"/>
            <circle cx="40" cy="40" r="3.5" fill="#4ade80"/>
        </svg>

        <h1>GAIA</h1>
        <p class="tagline">
            A <strong>self-learning</strong> platform for disease research.
            Scan a genome, discover its grammar, map variants, screen compounds,
            and design a protocol — <strong>end to end</strong>.
        </p>

        <div class="hero-cta">
            <a href="#learning" class="btn btn-primary">How it learns →</a>
            <a href="https://github.com/ObviousSatire/GaiaAI" class="btn">View source</a>
        </div>

        <div class="stats">
            <div class="stat">
                <div class="num" data-count="1081166" data-format="k">0</div>
                <div class="label">Variant mappings</div>
            </div>
            <div class="stat">
                <div class="num" data-count="56" data-format="plus">0</div>
                <div class="label">Genome features</div>
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
        <h2>What <span class="accent">GAIA</span> is</h2>
        <p class="lead">
            A two-layer self-learning stack for computational drug discovery.
            One layer learns the grammar of the genome. The other learns the
            grammar of disease. Together they turn raw sequence into a
            treatment protocol.
        </p>
        <p style="color: var(--fg-dim); font-size: 1.05rem; line-height: 1.8;">
            Most drug discovery starts with a hypothesis and tests it. GAIA
            starts with the full genome — every variant, every gene, every
            pathway — and works backward. Nothing is hand-coded. Both layers
            improve as more labeled data arrives.
        </p>
    </div>
</section>

<section id="learning">
    <div class="container">
        <h2>How GAIA <span class="accent">learns</span></h2>
        <p class="lead">
            Two learning layers, connected by a shared interface. Each layer
            discovers structure from data. Neither is programmed with the
            answer.
        </p>

        <div class="learning-loop">
            <h3>Layer 1 — Genome grammar discovery</h3>
            <div class="loop-steps">
                <div class="loop-step">
                    <strong>Ingest raw sequence</strong>
                    Full chromosomes with labels from GENCODE (exon / intron / intergenic).
                </div>
                <div class="loop-step">
                    <strong>Extract features</strong>
                    Statistics per segment — entropy, GC content, motif scores, conservation.
                </div>
                <div class="loop-step">
                    <strong>Train classifier</strong>
                    Weights updated by gradient descent. Discovers which features predict which class.
                </div>
                <div class="loop-step">
                    <strong>Cross-validate</strong>
                    Train on one chromosome, test on another. If it holds, the grammar is universal.
                </div>
            </div>
            <p style="margin-top: 28px; color: var(--fg-dim); font-size: 0.95rem;">
                No hand-coded rules like "if GC > 0.55 then coding." The
                classifier discovers its own thresholds from data.
            </p>
        </div>

        <div class="learning-loop">
            <h3>Layer 2 — Function discovery</h3>
            <div class="loop-steps">
                <div class="loop-step">
                    <strong>Ingest mappings</strong>
                    Variant-to-disease pairs, compound-target bindings, protein structures.
                </div>
                <div class="loop-step">
                    <strong>Build graph</strong>
                    Variant → gene → pathway → disease → compound. Every new paper adds nodes and edges.
                </div>
                <div class="loop-step">
                    <strong>Predict</strong>
                    Query the graph, score candidates, rank outcomes.
                </div>
                <div class="loop-step">
                    <strong>Retrain</strong>
                    As more pairs are labeled, the classifier updates. Predictions improve.
                </div>
            </div>
            <p style="margin-top: 28px; color: var(--fg-dim); font-size: 0.95rem;">
                The graph grows automatically. The classifier retrains
                continuously. Cross-validation tests whether patterns are
                general or overfit.
            </p>
        </div>

        <div class="learning-loop">
            <h3>The loop between layers</h3>
            <div class="loop-steps">
                <div class="loop-step">
                    <strong>New variant arrives</strong>
                    GAIA queries the genome layer.
                </div>
                <div class="loop-step">
                    <strong>Structural features returned</strong>
                    Segment class, conservation, GC content, motif context.
                </div>
                <div class="loop-step">
                    <strong>Features join training data</strong>
                    GAIA's function classifier retrains with the new inputs.
                </div>
                <div class="loop-step">
                    <strong>Performance measured</strong>
                    If features help, F1 rises. If not, they're weighted down.
                </div>
            </div>
            <p style="margin-top: 28px; color: var(--fg-dim); font-size: 0.95rem;">
                The genome layer says "what does the sequence look like."
                GAIA's function layer says "what does it mean for disease."
                Both learn. Both improve.
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
                <p>Chaos-fractal analysis across whole chromosomes. Every window classified by fractal dimension, Hurst exponent, and GC content.</p>
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
                <p>Over 1 million population variants mapped to gene coordinates. Allele frequencies, functional context, and gene-level aggregation.</p>
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
                <p>Seven compound libraries — hundreds of thousands of purchasable small molecules, natural products, and known drugs.</p>
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
                <p>Ranked multi-compound protocol with predicted outcomes across time — reversal, function, risk, safety.</p>
            </div>
        </div>
    </div>
</section>

<section>
    <div class="container">
        <h2>What GAIA <span class="accent">does</span></h2>
        <p class="lead">Twelve integrated subsystems, from raw genome to treatment protocol.</p>

        <div class="capabilities">
            <div class="capability">
                <svg class="glyph" width="40" height="40" viewBox="0 0 40 40">
                    <circle cx="20" cy="20" r="16" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <path d="M8,20 Q20,12 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <path d="M8,20 Q20,28 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                </svg>
                <h3>Chaos-fractal genome scanner</h3>
                <p>Classifies every window of a chromosome by fractal dimension, Hurst exponent, and GC content. Identifies coding regions, conserved patterns, and structural signals across whole genomes.</p>
                <div class="tags"><span class="tag">genome</span><span class="tag">fractal</span><span class="tag">classification</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="40" height="40" viewBox="0 0 40 40">
                    <circle cx="12" cy="14" r="3" fill="#60a5fa"/>
                    <circle cx="28" cy="14" r="3" fill="#60a5fa"/>
                    <circle cx="20" cy="28" r="3" fill="#60a5fa"/>
                    <line x1="14" y1="14" x2="26" y2="14" stroke="#60a5fa" stroke-width="1.5"/>
                    <line x1="14" y1="16" x2="19" y2="25" stroke="#60a5fa" stroke-width="1.5"/>
                    <line x1="26" y1="16" x2="21" y2="25" stroke="#60a5fa" stroke-width="1.5"/>
                </svg>
                <h3>Variant-to-gene mapping</h3>
                <p>Over 1 million population variants mapped to gene coordinates. Allele frequencies, functional context, and gene-level aggregation at scale.</p>
                <div class="tags"><span class="tag">variants</span><span class="tag">genes</span><span class="tag">population</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="40" height="40" viewBox="0 0 40 40">
                    <circle cx="8" cy="20" r="2" fill="#a78bfa"/>
                    <circle cx="20" cy="8" r="2" fill="#a78bfa"/>
                    <circle cx="32" cy="20" r="2" fill="#a78bfa"/>
                    <circle cx="20" cy="32" r="2" fill="#a78bfa"/>
                    <line x1="8" y1="20" x2="20" y2="8" stroke="#a78bfa" stroke-width="1"/>
                    <line x1="20" y1="8" x2="32" y2="20" stroke="#a78bfa" stroke-width="1"/>
                    <line x1="32" y1="20" x2="20" y2="32" stroke="#a78bfa" stroke-width="1"/>
                    <line x1="20" y1="32" x2="8" y2="20" stroke="#a78bfa" stroke-width="1"/>
                </svg>
                <h3>Self-learning disease graph</h3>
                <p>GAIA ingests variant-to-disease mappings, compound-target bindings, and protein structures. It builds a graph that grows automatically as new papers publish. The classifier retrains continuously.</p>
                <div class="tags"><span class="tag">graph</span><span class="tag">self-learning</span><span class="tag">continuous</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="40" height="40" viewBox="0 0 40 40">
                    <rect x="4" y="14" width="9" height="9" rx="1.5" fill="#f472b6"/>
                    <rect x="15" y="14" width="9" height="9" rx="1.5" fill="#f472b6" opacity="0.75"/>
                    <rect x="26" y="14" width="9" height="9" rx="1.5" fill="#f472b6" opacity="0.5"/>
                </svg>
                <h3>Seven compound libraries</h3>
                <p>ZINC 3D, COCONUT natural products, ChEMBL bioactives, plus several other curated sources. Hundreds of thousands of purchasable and known compounds screened against any target.</p>
                <div class="tags"><span class="tag">screening</span><span class="tag">ZINC</span><span class="tag">COCONUT</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="40" height="40" viewBox="0 0 40 40">
                    <circle cx="20" cy="20" r="14" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="20" cy="20" r="7" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="20" cy="20" r="2.5" fill="#4ade80"/>
                    <line x1="20" y1="6" x2="20" y2="2" stroke="#4ade80" stroke-width="1.5"/>
                    <line x1="34" y1="20" x2="38" y2="20" stroke="#4ade80" stroke-width="1.5"/>
                </svg>
                <h3>Molecular physics engine</h3>
                <p>Nine methods in one canonical C++17 header — Lennard-Jones, Coulomb, Generalized Born, MM-GBSA, FEP, entropy, QM, water placement, Gasteiger charges. Zero external dependencies.</p>
                <div class="tags"><span class="tag">physics</span><span class="tag">C++17</span><span class="tag">self-contained</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="40" height="40" viewBox="0 0 40 40">
                    <path d="M6,32 L6,24 L14,24 L14,16 L22,16 L22,24 L30,24 L30,10 L34,10" fill="none" stroke="#60a5fa" stroke-width="2" stroke-linejoin="round"/>
                    <circle cx="6" cy="32" r="2" fill="#60a5fa"/>
                    <circle cx="34" cy="10" r="2" fill="#60a5fa"/>
                </svg>
                <h3>Protocol simulator</h3>
                <p>Simulates multi-compound protocols across time. Predicts damage reversal, function restoration, disease risk, and safety margins at 30, 90, 180, and 365 days.</p>
                <div class="tags"><span class="tag">simulation</span><span class="tag">multi-compound</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="40" height="40" viewBox="0 0 40 40">
                    <path d="M6,12 L6,28 M12,12 L12,28 M18,12 L18,28 M24,12 L24,28 M30,12 L30,28 M36,12 L36,28" stroke="#a78bfa" stroke-width="1.5"/>
                    <line x1="6" y1="12" x2="12" y2="18" stroke="#a78bfa" stroke-width="1.5"/>
                    <line x1="12" y1="18" x2="18" y2="12" stroke="#a78bfa" stroke-width="1.5"/>
                    <line x1="18" y1="12" x2="24" y2="18" stroke="#a78bfa" stroke-width="1.5"/>
                    <line x1="24" y1="18" x2="30" y2="12" stroke="#a78bfa" stroke-width="1.5"/>
                </svg>
                <h3>Link prediction</h3>
                <p>A trained classifier that predicts missing variant-gene-pathway-disease links from graph structure. Improves automatically as the graph grows.</p>
                <div class="tags"><span class="tag">prediction</span><span class="tag">graph learning</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="40" height="40" viewBox="0 0 40 40">
                    <rect x="8" y="8" width="24" height="24" rx="3" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <line x1="14" y1="14" x2="26" y2="14" stroke="#4ade80" stroke-width="1.5"/>
                    <line x1="14" y1="20" x2="26" y2="20" stroke="#4ade80" stroke-width="1.5"/>
                    <line x1="14" y1="26" x2="20" y2="26" stroke="#4ade80" stroke-width="1.5"/>
                </svg>
                <h3>Reproducible datasets</h3>
                <p>Every dataset archived on Zenodo with permanent DOIs. Over 380 GB of raw inputs, intermediate results, and benchmarks — reproducible from public sources.</p>
                <div class="tags"><span class="tag">Zenodo</span><span class="tag">DOIs</span><span class="tag">reproducible</span></div>
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
            <tr><th>Dataset</th><th>Size</th><th>Contents</th><th>DOI</th></tr>
            <tr><td>Compound library I</td><td>25.7 GB</td><td>ZINC shards</td><td><a href="https://doi.org/10.5281/zenodo.22949286">22949286</a></td></tr>
            <tr><td>Compound library II</td><td>44.3 GB</td><td>ZINC compound set</td><td><a href="https://doi.org/10.5281/zenodo.23110910">23110910</a></td></tr>
            <tr><td>Compound library III</td><td>45.1 GB</td><td>ZINC compound set</td><td><a href="https://doi.org/10.5281/zenodo.23124533">23124533</a></td></tr>
            <tr><td>Compound library IV</td><td>93.7 GB</td><td>ZINC compound set</td><td><a href="https://doi.org/10.5281/zenodo.23127161">23127161</a></td></tr>
            <tr><td>Compound library V</td><td>128.7 GB</td><td>ZINC compound set</td><td><a href="https://doi.org/10.5281/zenodo.23139933">23139933</a></td></tr>
            <tr><td>Benchmarks</td><td>20 GB</td><td>PDBbind, DUD-E, FEP+</td><td><a href="https://doi.org/10.5281/zenodo.22946723">22946723</a></td></tr>
        </table>
    </div>
</section>

<footer>
    <div class="container">
        <div class="footer-links">
            <a href="https://github.com/ObviousSatire/GaiaAI">Source on GitHub</a>
            <a href="https://doi.org/10.5281/zenodo.22949286">Zenodo datasets</a>
            <a href="#learning">Self-learning</a>
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

// Section fade-in
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

// Hero parallax
const heroBg = document.querySelector('.hero-bg');
if (heroBg) {
    window.addEventListener('scroll', () => {
        const y = window.scrollY;
        if (y < window.innerHeight) {
            heroBg.style.transform = `translateY(${y * 0.35}px) scale(${1 + y * 0.0003})`;
        }
    }, { passive: true });
}
</script>

</body>
</html>
