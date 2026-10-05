---
layout: null
---
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GAIA — Self-Learning Platform for Disease Research</title>
<meta name="description" content="A self-learning platform for computational disease research. Scans genomes, scans the web, and builds knowledge that grows.">
<link rel="stylesheet" href="assets/style.css">
</head>
<body>

<div class="hero">
    <svg class="hero-bg" viewBox="0 0 1800 900" preserveAspectRatio="xMidYMid slice">
        <defs>
            <linearGradient id="helixGrad" x1="0%" y1="0%" x2="100%" y2="0%">
                <stop offset="0%" stop-color="#a7f3d0" stop-opacity="0.7"/>
                <stop offset="33%" stop-color="#4ade80" stop-opacity="0.7"/>
                <stop offset="66%" stop-color="#34d399" stop-opacity="0.7"/>
                <stop offset="100%" stop-color="#60a5fa" stop-opacity="0.7"/>
            </linearGradient>
            <radialGradient id="cellGlow" cx="50%" cy="50%" r="50%">
                <stop offset="0%" stop-color="#4ade80" stop-opacity="0.3"/>
                <stop offset="100%" stop-color="#4ade80" stop-opacity="0"/>
            </radialGradient>
        </defs>

        <!-- Background organic cells -->
        <circle class="cell-pulse" cx="200" cy="150" r="80" fill="url(#cellGlow)"/>
        <circle class="cell-pulse" cx="1600" cy="700" r="120" fill="url(#cellGlow)"/>
        <circle class="cell-pulse" cx="1200" cy="200" r="60" fill="url(#cellGlow)"/>

        <!-- Vines -->
        <g class="vine-sway" opacity="0.4">
            <path d="M100,900 Q150,700 80,500 Q140,300 100,100" stroke="#4ade80" stroke-width="1.5" fill="none"/>
            <path d="M100,900 Q150,700 80,500 Q140,300 100,100" stroke="#a7f3d0" stroke-width="0.5" fill="none" opacity="0.5" transform="translate(4,0)"/>
        </g>
        <g class="vine-sway" opacity="0.35">
            <path d="M1700,900 Q1650,700 1720,500 Q1660,300 1700,100" stroke="#34d399" stroke-width="1.5" fill="none"/>
        </g>
        <g class="vine-sway" opacity="0.3">
            <path d="M500,900 Q550,750 480,600 Q540,450 500,300" stroke="#60a5fa" stroke-width="1" fill="none"/>
        </g>
        <g class="vine-sway" opacity="0.3">
            <path d="M1300,900 Q1250,750 1320,600 Q1260,450 1300,300" stroke="#4ade80" stroke-width="1" fill="none"/>
        </g>

        <!-- Animated DNA helix -->
        <g class="helix-flow" transform="translate(900, 450)">
            <path d="M-1200,0 Q-600,-220 0,0 T1200,0" stroke="url(#helixGrad)" stroke-width="1.8" fill="none"/>
            <path d="M-1200,0 Q-600,220 0,0 T1200,0" stroke="url(#helixGrad)" stroke-width="1.8" fill="none"/>
            <path d="M-1100,40 Q-600,-180 0,40 T1100,40" stroke="url(#helixGrad)" stroke-width="1" fill="none" opacity="0.5"/>
            <path d="M-1100,-40 Q-600,180 0,-40 T1100,-40" stroke="url(#helixGrad)" stroke-width="1" fill="none" opacity="0.5"/>
        </g>

        <!-- Floating particles -->
        <g>
            <circle class="particle" cx="200" cy="200" r="3" fill="#4ade80"/>
            <circle class="particle" cx="500" cy="680" r="2.5" fill="#a7f3d0"/>
            <circle class="particle" cx="1400" cy="180" r="3" fill="#34d399"/>
            <circle class="particle" cx="1650" cy="580" r="2.5" fill="#60a5fa"/>
            <circle class="particle" cx="900" cy="100" r="3" fill="#4ade80"/>
            <circle class="particle" cx="300" cy="500" r="2.5" fill="#a7f3d0"/>
            <circle class="particle" cx="1500" cy="420" r="3" fill="#4ade80"/>
            <circle class="particle" cx="700" cy="780" r="2.5" fill="#60a5fa"/>
            <circle class="particle" cx="1100" cy="720" r="3" fill="#34d399"/>
            <circle class="particle" cx="600" cy="300" r="2.5" fill="#a7f3d0"/>
            <circle class="particle" cx="1250" cy="350" r="3" fill="#4ade80"/>
            <circle class="particle" cx="350" cy="380" r="2.5" fill="#60a5fa"/>
        </g>
    </svg>

    <div class="container hero-content">
        <svg class="hero-logo" width="90" height="90" viewBox="0 0 80 80">
            <defs>
                <linearGradient id="logoGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                    <stop offset="0%" stop-color="#a7f3d0"/>
                    <stop offset="50%" stop-color="#4ade80"/>
                    <stop offset="100%" stop-color="#34d399"/>
                </linearGradient>
            </defs>
            <circle class="ring" cx="40" cy="40" r="36" fill="none" stroke="url(#logoGrad)" stroke-width="2"/>
            <path d="M22,40 Q40,18 58,40 T22,40" fill="none" stroke="url(#logoGrad)" stroke-width="2"/>
            <path d="M22,40 Q40,62 58,40 T22,40" fill="none" stroke="url(#logoGrad)" stroke-width="2"/>
            <circle cx="40" cy="40" r="4" fill="#4ade80"/>
            <circle cx="40" cy="40" r="8" fill="none" stroke="#4ade80" stroke-width="0.5" opacity="0.5"/>
        </svg>

        <h1>GAIA</h1>
        <p class="tagline">
            A <strong>self-learning</strong> platform for disease research.
            It reads the genome, reads the web, and grows into something
            that knows more tomorrow than it did today.
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
                <div class="label">Scoring methods</div>
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
        <svg class="divider-leaf" width="40" height="40" viewBox="0 0 40 40">
            <path d="M20,4 Q32,12 20,20 Q8,12 20,4 Z" fill="none" stroke="#4ade80" stroke-width="1.5" opacity="0.7"/>
            <path d="M20,20 Q32,28 20,36 Q8,28 20,20 Z" fill="none" stroke="#4ade80" stroke-width="1.5" opacity="0.7"/>
        </svg>
        <h2>What <span class="accent">GAIA</span> is</h2>
        <p class="lead">
            Two learning systems, connected. One reads the language of the
            genome. The other reads the language of disease. Both improve
            continuously as new data arrives — from files, from databases,
            and from the open web.
        </p>
        <p style="color: var(--fg-dim); font-size: 1.05rem; line-height: 1.8;">
            Most drug discovery starts with a hypothesis and tests it. GAIA
            starts with the raw genome and the raw literature, and works
            backward. Nothing is hand-coded. Both layers discover their own
            patterns.
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
            <h3>Layer 1 — Reading the genome</h3>
            <div class="loop-steps">
                <div class="loop-step">
                    <strong>Ingest raw sequence</strong>
                    Full chromosomes with labels from curated gene databases.
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
        </div>

        <div class="learning-loop">
            <h3>Layer 2 — Reading the world</h3>
            <div class="loop-steps">
                <div class="loop-step">
                    <strong>Ingest mappings</strong>
                    Variant-to-disease pairs, compound-target bindings, protein structures.
                </div>
                <div class="loop-step">
                    <strong>Build graph</strong>
                    Variant → gene → pathway → disease → compound. Every new source adds nodes and edges.
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
                    The disease classifier retrains with the new inputs.
                </div>
                <div class="loop-step">
                    <strong>Performance measured</strong>
                    If features help, prediction improves. If not, they fade.
                </div>
            </div>
        </div>
    </div>
</section>

<section id="sources">
    <div class="container">
        <h2>It reads the <span class="accent">open web</span></h2>
        <p class="lead">
            GAIA doesn't wait for someone to hand it data. It crawls hundreds
            of curated sources — papers, repositories, databases, trial
            registries — and grows its knowledge graph as new findings are
            published.
        </p>

        <div class="sources-hero">
            <div class="sources-visual">
                <svg viewBox="0 0 400 420" preserveAspectRatio="xMidYMid meet">
                    <defs>
                        <radialGradient id="hubGlow" cx="50%" cy="50%" r="50%">
                            <stop offset="0%" stop-color="#4ade80" stop-opacity="0.9"/>
                            <stop offset="100%" stop-color="#4ade80" stop-opacity="0"/>
                        </radialGradient>
                    </defs>

                    <!-- Central hub -->
                    <circle cx="200" cy="210" r="70" fill="url(#hubGlow)" opacity="0.4"/>
                    <circle cx="200" cy="210" r="45" fill="none" stroke="#4ade80" stroke-width="2"/>
                    <circle cx="200" cy="210" r="55" fill="none" stroke="#4ade80" stroke-width="0.5" opacity="0.5"/>
                    <text x="200" y="216" text-anchor="middle" font-family="monospace" font-size="16" fill="#4ade80" font-weight="bold">GAIA</text>

                    <!-- Source nodes -->
                    <g>
                        <circle class="node-pulse" cx="60" cy="60" r="6" fill="#60a5fa"/>
                        <text x="60" y="42" text-anchor="middle" font-size="9" fill="#8fa89c">Publications</text>
                        <line class="link-draw" x1="60" y1="60" x2="200" y2="210" stroke="#60a5fa" stroke-width="1" opacity="0.4"/>
                    </g>
                    <g>
                        <circle class="node-pulse" cx="340" cy="60" r="6" fill="#a7f3d0"/>
                        <text x="340" y="42" text-anchor="middle" font-size="9" fill="#8fa89c">Genomes</text>
                        <line class="link-draw" x1="340" y1="60" x2="200" y2="210" stroke="#a7f3d0" stroke-width="1" opacity="0.4"/>
                    </g>
                    <g>
                        <circle class="node-pulse" cx="60" cy="210" r="6" fill="#34d399"/>
                        <text x="60" y="192" text-anchor="middle" font-size="9" fill="#8fa89c">Proteins</text>
                        <line class="link-draw" x1="60" y1="210" x2="200" y2="210" stroke="#34d399" stroke-width="1" opacity="0.4"/>
                    </g>
                    <g>
                        <circle class="node-pulse" cx="340" cy="210" r="6" fill="#4ade80"/>
                        <text x="340" y="192" text-anchor="middle" font-size="9" fill="#8fa89c">Variants</text>
                        <line class="link-draw" x1="340" y1="210" x2="200" y2="210" stroke="#4ade80" stroke-width="1" opacity="0.4"/>
                    </g>
                    <g>
                        <circle class="node-pulse" cx="60" cy="360" r="6" fill="#60a5fa"/>
                        <text x="60" y="342" text-anchor="middle" font-size="9" fill="#8fa89c">Compounds</text>
                        <line class="link-draw" x1="60" y1="360" x2="200" y2="210" stroke="#60a5fa" stroke-width="1" opacity="0.4"/>
                    </g>
                    <g>
                        <circle class="node-pulse" cx="340" cy="360" r="6" fill="#a7f3d0"/>
                        <text x="340" y="342" text-anchor="middle" font-size="9" fill="#8fa89c">Trials</text>
                        <line class="link-draw" x1="340" y1="360" x2="200" y2="210" stroke="#a7f3d0" stroke-width="1" opacity="0.4"/>
                    </g>
                    <g>
                        <circle class="node-pulse" cx="200" cy="60" r="6" fill="#34d399"/>
                        <text x="200" y="42" text-anchor="middle" font-size="9" fill="#8fa89c">Pathways</text>
                        <line class="link-draw" x1="200" y1="60" x2="200" y2="210" stroke="#34d399" stroke-width="1" opacity="0.4"/>
                    </g>
                    <g>
                        <circle class="node-pulse" cx="200" cy="360" r="6" fill="#4ade80"/>
                        <text x="200" y="342" text-anchor="middle" font-size="9" fill="#8fa89c">Structures</text>
                        <line class="link-draw" x1="200" y1="360" x2="200" y2="210" stroke="#4ade80" stroke-width="1" opacity="0.4"/>
                    </g>
                </svg>
            </div>

            <div class="sources-list">
                <div class="source-category">
                    <div class="label">Scientific literature</div>
                    <div class="desc">Curated feed of papers on variants, disease associations, and compound activity.</div>
                </div>
                <div class="source-category">
                    <div class="label">Reference genomes</div>
                    <div class="desc">Human assemblies, gene annotations, and regulatory maps. The base layer for genome scanning.</div>
                </div>
                <div class="source-category">
                    <div class="label">Population variants</div>
                    <div class="desc">Clinical significance and population frequencies. Every new variant adds evidence.</div>
                </div>
                <div class="source-category">
                    <div class="label">Protein structures</div>
                    <div class="desc">Structures, sequences, functions. The docking targets and their interaction partners.</div>
                </div>
                <div class="source-category">
                    <div class="label">Compound libraries</div>
                    <div class="desc">Bioactivity data, purchasable molecules, natural products. The screening universe.</div>
                </div>
                <div class="source-category">
                    <div class="label">Clinical registries</div>
                    <div class="desc">Trial registries, outcomes, adverse events. Evidence that informs protocol design.</div>
                </div>
            </div>
        </div>

        <div class="scan-visual">
            <h3>The continuous loop</h3>
            <div class="scan-flow">
                <div class="scan-step">
                    <span class="icon">🌐</span>
                    <div class="label">Crawl</div>
                    <div class="desc">Poll curated sources</div>
                </div>
                <div class="scan-step">
                    <span class="icon">📖</span>
                    <div class="label">Parse</div>
                    <div class="desc">Extract entities, relations</div>
                </div>
                <div class="scan-step">
                    <span class="icon">✓</span>
                    <div class="label">Validate</div>
                    <div class="desc">Cross-check across sources</div>
                </div>
                <div class="scan-step">
                    <span class="icon">🌱</span>
                    <div class="label">Integrate</div>
                    <div class="desc">Grow the knowledge graph</div>
                </div>
                <div class="scan-step">
                    <span class="icon">📈</span>
                    <div class="label">Retrain</div>
                    <div class="desc">Learn from the new evidence</div>
                </div>
            </div>
        </div>
    </div>
</section>

<section id="pipeline">
    <div class="container">
        <h2>The <span class="accent">pipeline</span></h2>
        <p class="lead">From raw genome to treatment protocol, in five stages.</p>

        <div class="pipeline">
            <div class="stage">
                <div class="stage-num">STAGE 01</div>
                <svg width="44" height="44" viewBox="0 0 40 40">
                    <circle cx="20" cy="20" r="16" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <path d="M8,20 Q20,10 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <path d="M8,20 Q20,30 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                </svg>
                <h3>Read the genome</h3>
                <p>Every window classified by structural signature — coding, conserved, regulatory, or silent.</p>
            </div>
            <div class="stage">
                <div class="stage-num">STAGE 02</div>
                <svg width="44" height="44" viewBox="0 0 40 40">
                    <circle cx="10" cy="20" r="4" fill="#60a5fa"/>
                    <circle cx="30" cy="20" r="4" fill="#60a5fa"/>
                    <line x1="14" y1="20" x2="26" y2="20" stroke="#60a5fa" stroke-width="1.5"/>
                    <line x1="10" y1="16" x2="10" y2="10" stroke="#60a5fa" stroke-width="1.5"/>
                    <line x1="30" y1="24" x2="30" y2="30" stroke="#60a5fa" stroke-width="1.5"/>
                </svg>
                <h3>Map the variants</h3>
                <p>Population variation placed in context. Every variant associated with its gene, pathway, and evidence.</p>
            </div>
            <div class="stage">
                <div class="stage-num">STAGE 03</div>
                <svg width="44" height="44" viewBox="0 0 40 40">
                    <rect x="8" y="12" width="24" height="16" rx="3" fill="none" stroke="#a7f3d0" stroke-width="1.5"/>
                    <line x1="14" y1="12" x2="14" y2="8" stroke="#a7f3d0" stroke-width="1.5"/>
                    <line x1="26" y1="12" x2="26" y2="8" stroke="#a7f3d0" stroke-width="1.5"/>
                    <circle cx="20" cy="20" r="3" fill="#a7f3d0"/>
                </svg>
                <h3>Screen the compounds</h3>
                <p>Multiple libraries of small molecules and natural products, ranked by binding potential.</p>
            </div>
            <div class="stage">
                <div class="stage-num">STAGE 04</div>
                <svg width="44" height="44" viewBox="0 0 40 40">
                    <path d="M20,4 L36,14 L36,26 L20,36 L4,26 L4,14 Z" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="20" cy="20" r="4" fill="#4ade80"/>
                </svg>
                <h3>Score every interaction</h3>
                <p>Multiple scoring approaches combined into one ranking. Physical, chemical, and contextual.</p>
            </div>
            <div class="stage">
                <div class="stage-num">STAGE 05</div>
                <svg width="44" height="44" viewBox="0 0 40 40">
                    <path d="M8,20 L16,28 L32,12" fill="none" stroke="#60a5fa" stroke-width="2.5" stroke-linecap="round"/>
                </svg>
                <h3>Design the protocol</h3>
                <p>Multi-compound protocol with predicted outcomes across time. One ranking, one plan.</p>
            </div>
        </div>
    </div>
</section>

<section id="math">
    <div class="container">
        <h2>The <span class="accent">math</span> behind the learning</h2>
        <p class="lead">
            Both layers learn from data, not rules. These are the formulas
            each layer uses to update itself.
        </p>

        <div class="math-grid">
            <div class="math-card">
                <h3>Shannon entropy</h3>
                <div class="sub">Information density per window</div>
                <div class="formula">
                    <span class="var">H</span> <span class="op">=</span> <span class="op">−</span> <span class="fn">Σ</span> <span class="var">p</span><sub>i</sub> <span class="fn">log</span><sub>2</sub> <span class="var">p</span><sub>i</sub>
                </div>
                <p>Measures the information density of a DNA window. Low entropy = repeats. High entropy = information-rich regions.</p>
            </div>

            <div class="math-card">
                <h3>Fractal dimension</h3>
                <div class="sub">How structure fills space across scales</div>
                <div class="formula">
                    <span class="var">D</span> <span class="op">=</span> <span class="fn">lim</span><sub>ε→0</sub> <span class="fn">log</span> <span class="var">N</span>(<span class="var">ε</span>) <span class="op">/</span> <span class="fn">log</span>(1/<span class="var">ε</span>)
                </div>
                <p>How the sequence fills space across scales. Coding regions cluster around a distinctive signature.</p>
            </div>

            <div class="math-card">
                <h3>Hurst exponent</h3>
                <div class="sub">Long-range correlation signal</div>
                <div class="formula">
                    <span class="fn">E</span>[<span class="var">R</span>(<span class="var">n</span>)/<span class="var">S</span>(<span class="var">n</span>)] <span class="op">~</span> <span class="var">c</span> <span class="op">·</span> <span class="var">n</span><sup><span class="var">H</span></sup>
                </div>
                <p>Detects whether a window shows persistent or anti-persistent structure. Independent of GC content.</p>
            </div>

            <div class="math-card">
                <h3>Class probability</h3>
                <div class="sub">Which features predict which class</div>
                <div class="formula">
                    <span class="var">P</span>(<span class="var">c</span> | <span class="var">x</span>) <span class="op">=</span> <span class="var">P</span>(<span class="var">x</span> | <span class="var">c</span>) <span class="op">·</span> <span class="var">P</span>(<span class="var">c</span>) <span class="op">/</span> <span class="var">P</span>(<span class="var">x</span>)
                </div>
                <p>Given a segment's features, what's the probability it belongs to each class? Updates as new data arrives.</p>
            </div>

            <div class="math-card">
                <h3>Gradient descent</h3>
                <div class="sub">How weights change with each example</div>
                <div class="formula">
                    <span class="var">w</span><sub>t+1</sub> <span class="op">=</span> <span class="var">w</span><sub>t</sub> <span class="op">−</span> <span class="var">η</span> <span class="op">·</span> <span class="fn">∇</span><span class="var">L</span>(<span class="var">w</span><sub>t</sub>)
                </div>
                <p>Weights move downhill on the loss surface. The learning rate controls how fast.</p>
            </div>

            <div class="math-card">
                <h3>Cross-validated F1</h3>
                <div class="sub">Generalization, not memorization</div>
                <div class="formula">
                    <span class="var">F</span><sub>1</sub> <span class="op">=</span> 2 <span class="op">·</span> <span class="var">P</span> <span class="op">·</span> <span class="var">R</span> <span class="op">/</span> (<span class="var">P</span> <span class="op">+</span> <span class="var">R</span>)
                </div>
                <p>Precision × recall balance. Train on one chromosome, test on another. If F1 holds, the pattern is universal.</p>
            </div>

            <div class="math-card">
                <h3>Pairwise interaction energy</h3>
                <div class="sub">Attraction and repulsion between atoms</div>
                <div class="formula">
                    <span class="var">E</span> <span class="op">=</span> 4<span class="var">ε</span> [ (<span class="var">σ</span>/<span class="var">r</span>)<sup>12</sup> <span class="op">−</span> (<span class="var">σ</span>/<span class="var">r</span>)<sup>6</sup> ]
                </div>
                <p>One term for repulsion, one for attraction. Every docking score starts here.</p>
            </div>

            <div class="math-card">
                <h3>Screened electrostatics</h3>
                <div class="sub">Charges interacting at distance</div>
                <div class="formula">
                    <span class="var">E</span> <span class="op">=</span> 332 <span class="op">·</span> <span class="var">q</span><sub>i</sub> <span class="var">q</span><sub>j</sub> <span class="op">·</span> <span class="fn">e</span><sup>−<span class="var">κr</span></sup> <span class="op">/</span> <span class="var">r</span>
                </div>
                <p>Charges attract or repel. Salt in solution screens the interaction at distance.</p>
            </div>

            <div class="math-card">
                <h3>Charge equilibration</h3>
                <div class="sub">How electrons redistribute along bonds</div>
                <div class="formula">
                    <span class="var">χ</span><sub>i</sub> <span class="op">←</span> <span class="var">χ</span><sub>i</sub> <span class="op">+</span> <span class="var">η</span> <span class="op">·</span> <span class="var">q</span><sub>i</sub> <span class="op">+</span> <span class="op">Σ</span> <span class="var">γ</span><sub>ij</sub> <span class="var">q</span><sub>j</sub>
                </div>
                <p>Charge flows between bonded atoms until electronegativity equilibrates across the molecule.</p>
            </div>
        </div>
    </div>
</section>

<section id="capabilities">
    <div class="container">
        <h2>What it <span class="accent">does</span></h2>
        <p class="lead">Multiple systems working together. From raw signal to a plan.</p>

        <div class="capabilities">
            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <circle cx="20" cy="20" r="16" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <path d="M8,20 Q20,12 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <path d="M8,20 Q20,28 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                </svg>
                <h3>Genome scanning</h3>
                <p>Every window of a chromosome classified by its structural signature. Coding regions, conserved patterns, regulatory signals — all identified from raw sequence.</p>
                <div class="tags"><span class="tag">genome</span><span class="tag">structure</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <circle cx="12" cy="14" r="3" fill="#60a5fa"/>
                    <circle cx="28" cy="14" r="3" fill="#60a5fa"/>
                    <circle cx="20" cy="28" r="3" fill="#60a5fa"/>
                    <line x1="14" y1="14" x2="26" y2="14" stroke="#60a5fa" stroke-width="1.5"/>
                    <line x1="14" y1="16" x2="19" y2="25" stroke="#60a5fa" stroke-width="1.5"/>
                    <line x1="26" y1="16" x2="21" y2="25" stroke="#60a5fa" stroke-width="1.5"/>
                </svg>
                <h3>Variant mapping</h3>
                <p>Population variation placed in context. Each variant tied to gene, pathway, and any known associations. The base layer of the knowledge graph.</p>
                <div class="tags"><span class="tag">variants</span><span class="tag">population</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <circle cx="8" cy="20" r="2.5" fill="#a7f3d0"/>
                    <circle cx="20" cy="8" r="2.5" fill="#a7f3d0"/>
                    <circle cx="32" cy="20" r="2.5" fill="#a7f3d0"/>
                    <circle cx="20" cy="32" r="2.5" fill="#a7f3d0"/>
                    <line x1="8" y1="20" x2="20" y2="8" stroke="#a7f3d0" stroke-width="1"/>
                    <line x1="20" y1="8" x2="32" y2="20" stroke="#a7f3d0" stroke-width="1"/>
                    <line x1="32" y1="20" x2="20" y2="32" stroke="#a7f3d0" stroke-width="1"/>
                    <line x1="20" y1="32" x2="8" y2="20" stroke="#a7f3d0" stroke-width="1"/>
                </svg>
                <h3>Knowledge graph</h3>
                <p>A growing network of variants, genes, pathways, diseases, and compounds. Every new source adds edges. The graph learns as the field publishes.</p>
                <div class="tags"><span class="tag">graph</span><span class="tag">continuous</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <rect x="4" y="14" width="9" height="9" rx="1.5" fill="#34d399"/>
                    <rect x="15" y="14" width="9" height="9" rx="1.5" fill="#34d399" opacity="0.7"/>
                    <rect x="26" y="14" width="9" height="9" rx="1.5" fill="#34d399" opacity="0.5"/>
                </svg>
                <h3>Compound libraries</h3>
                <p>Multiple curated libraries of small molecules and natural products. Thousands upon thousands of candidates ready to be screened against any target.</p>
                <div class="tags"><span class="tag">screening</span><span class="tag">molecules</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <circle cx="20" cy="20" r="14" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="20" cy="20" r="7" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="20" cy="20" r="2.5" fill="#4ade80"/>
                    <line x1="20" y1="6" x2="20" y2="2" stroke="#4ade80" stroke-width="1.5"/>
                    <line x1="34" y1="20" x2="38" y2="20" stroke="#4ade80" stroke-width="1.5"/>
                </svg>
                <h3>Interaction scoring</h3>
                <p>Multiple scoring approaches combined into one ranking. Physical, chemical, and contextual evidence rolled into a single number.</p>
                <div class="tags"><span class="tag">scoring</span><span class="tag">ranking</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <path d="M6,32 L6,24 L14,24 L14,16 L22,16 L22,24 L30,24 L30,10 L34,10" fill="none" stroke="#60a5fa" stroke-width="2" stroke-linejoin="round"/>
                    <circle cx="6" cy="32" r="2" fill="#60a5fa"/>
                    <circle cx="34" cy="10" r="2" fill="#60a5fa"/>
                </svg>
                <h3>Protocol design</h3>
                <p>Simulated multi-compound protocols across time. Predicted outcomes, risks, and safety margins — all in one plan.</p>
                <div class="tags"><span class="tag">simulation</span><span class="tag">planning</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <path d="M6,12 L6,28 M12,12 L12,28 M18,12 L18,28 M24,12 L24,28 M30,12 L30,28 M36,12 L36,28" stroke="#a7f3d0" stroke-width="1.5"/>
                    <line x1="6" y1="12" x2="12" y2="18" stroke="#a7f3d0" stroke-width="1.5"/>
                    <line x1="12" y1="18" x2="18" y2="12" stroke="#a7f3d0" stroke-width="1.5"/>
                    <line x1="18" y1="12" x2="24" y2="18" stroke="#a7f3d0" stroke-width="1.5"/>
                    <line x1="24" y1="18" x2="30" y2="12" stroke="#a7f3d0" stroke-width="1.5"/>
                </svg>
                <h3>Link prediction</h3>
                <p>A trained classifier that predicts missing links in the graph. Improves automatically as the graph grows.</p>
                <div class="tags"><span class="tag">prediction</span><span class="tag">self-learning</span></div>
            </div>

            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <rect x="8" y="8" width="24" height="24" rx="3" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <line x1="14" y1="14" x2="26" y2="14" stroke="#4ade80" stroke-width="1.5"/>
                    <line x1="14" y1="20" x2="26" y2="20" stroke="#4ade80" stroke-width="1.5"/>
                    <line x1="14" y1="26" x2="20" y2="26" stroke="#4ade80" stroke-width="1.5"/>
                </svg>
                <h3>Open datasets</h3>
                <p>Every stage archived publicly with permanent identifiers. The full pipeline, reproducible from raw public sources.</p>
                <div class="tags"><span class="tag">open</span><span class="tag">reproducible</span></div>
            </div>
        </div>
    </div>
</section>

<section id="scoring">
    <div class="container">
        <h2>Nine <span class="accent">scoring approaches</span>, one answer</h2>
        <p class="lead">
            Every compound-target pair is evaluated by multiple independent
            methods. Each contributes a piece. Together they produce one
            ranking.
        </p>

        <div class="scoring-grid">
            <div class="scoring-item">
                <svg width="36" height="36" viewBox="0 0 24 24"><circle cx="12" cy="12" r="3" fill="#4ade80"/><circle cx="4" cy="4" r="2" fill="#4ade80" opacity="0.5"/><circle cx="20" cy="4" r="2" fill="#4ade80" opacity="0.5"/><circle cx="4" cy="20" r="2" fill="#4ade80" opacity="0.5"/><circle cx="20" cy="20" r="2" fill="#4ade80" opacity="0.5"/></svg>
                <div class="name">Atom-atom</div>
                <div class="desc">Repulsion and attraction between every pair</div>
            </div>
            <div class="scoring-item">
                <svg width="36" height="36" viewBox="0 0 24 24"><ellipse cx="12" cy="12" rx="10" ry="6" fill="none" stroke="#34d399" stroke-width="1.5"/><circle cx="12" cy="12" r="3" fill="#34d399"/></svg>
                <div class="name">Solvent</div>
                <div class="desc">How water reshapes the interaction</div>
            </div>
            <div class="scoring-item">
                <svg width="36" height="36" viewBox="0 0 24 24"><path d="M2,12 Q12,4 22,12 Q12,20 2,12" fill="none" stroke="#a7f3d0" stroke-width="1.5"/><circle cx="12" cy="12" r="2" fill="#a7f3d0"/></svg>
                <div class="name">Binding energy</div>
                <div class="desc">The composite free-energy estimate</div>
            </div>
            <div class="scoring-item">
                <svg width="36" height="36" viewBox="0 0 24 24"><path d="M2,18 L6,12 L10,16 L14,8 L18,14 L22,6" fill="none" stroke="#60a5fa" stroke-width="1.5"/></svg>
                <div class="name">Perturbation</div>
                <div class="desc">How the energy changes along a path</div>
            </div>
            <div class="scoring-item">
                <svg width="36" height="36" viewBox="0 0 24 24"><path d="M12,4 Q16,12 12,20 Q8,12 12,4" fill="none" stroke="#4ade80" stroke-width="1.5"/><path d="M4,12 Q12,8 20,12 Q12,16 4,12" fill="none" stroke="#4ade80" stroke-width="1.5"/></svg>
                <div class="name">Disorder</div>
                <div class="desc">Entropy of the bound state</div>
            </div>
            <div class="scoring-item">
                <svg width="36" height="36" viewBox="0 0 24 24"><circle cx="12" cy="12" r="4" fill="none" stroke="#a7f3d0" stroke-width="1.5"/><ellipse cx="12" cy="12" rx="10" ry="4" fill="none" stroke="#a7f3d0" stroke-width="1"/><ellipse cx="12" cy="12" rx="4" ry="10" fill="none" stroke="#a7f3d0" stroke-width="1"/></svg>
                <div class="name">Quantum</div>
                <div class="desc">Electronic corrections on top</div>
            </div>
            <div class="scoring-item">
                <svg width="36" height="36" viewBox="0 0 24 24"><circle cx="12" cy="14" r="4" fill="none" stroke="#34d399" stroke-width="1.5"/><path d="M8,10 Q12,4 16,10" fill="none" stroke="#34d399" stroke-width="1.5"/></svg>
                <div class="name">Water placement</div>
                <div class="desc">Where waters sit in the pocket</div>
            </div>
            <div class="scoring-item">
                <svg width="36" height="36" viewBox="0 0 24 24"><path d="M4,12 L8,12 L10,6 L14,18 L16,12 L20,12" fill="none" stroke="#60a5fa" stroke-width="1.5"/></svg>
                <div class="name">Charge distribution</div>
                <div class="desc">How charge sits on each molecule</div>
            </div>
            <div class="scoring-item">
                <svg width="36" height="36" viewBox="0 0 24 24"><circle cx="7" cy="12" r="3" fill="none" stroke="#a7f3d0" stroke-width="1.5"/><circle cx="17" cy="12" r="3" fill="none" stroke="#a7f3d0" stroke-width="1.5"/><line x1="10" y1="12" x2="14" y2="12" stroke="#a7f3d0" stroke-width="1.5"/></svg>
                <div class="name">Geometry</div>
                <div class="desc">Hydrogen positions and bond angles</div>
            </div>
        </div>
    </div>
</section>

<section>
    <div class="container">
        <h2>Open <span class="accent">datasets</span></h2>
        <p class="lead">
            Every stage archived publicly with permanent identifiers.
            Reproducible from raw public sources.
        </p>

        <table class="data-table">
            <tr><th>Dataset</th><th>Size</th><th>Contents</th><th>Identifier</th></tr>
            <tr><td>Compound library I</td><td>25.7 GB</td><td>Screening shards</td><td><a href="https://doi.org/10.5281/zenodo.22949286">22949286</a></td></tr>
            <tr><td>Compound library II</td><td>44.3 GB</td><td>Compound set</td><td><a href="https://doi.org/10.5281/zenodo.23110910">23110910</a></td></tr>
            <tr><td>Compound library III</td><td>45.1 GB</td><td>Compound set</td><td><a href="https://doi.org/10.5281/zenodo.23124533">23124533</a></td></tr>
            <tr><td>Compound library IV</td><td>93.7 GB</td><td>Compound set</td><td><a href="https://doi.org/10.5281/zenodo.23127161">23127161</a></td></tr>
            <tr><td>Compound library V</td><td>128.7 GB</td><td>Compound set</td><td><a href="https://doi.org/10.5281/zenodo.23139933">23139933</a></td></tr>
            <tr><td>Benchmarks</td><td>20 GB</td><td>Reference data</td><td><a href="https://doi.org/10.5281/zenodo.22946723">22946723</a></td></tr>
        </table>
    </div>
</section>

<footer>
    <div class="container">
        <svg class="divider-leaf" width="32" height="32" viewBox="0 0 40 40">
            <path d="M20,4 Q32,12 20,20 Q8,12 20,4 Z" fill="none" stroke="#4ade80" stroke-width="1.5" opacity="0.6"/>
            <path d="M20,20 Q32,28 20,36 Q8,28 20,20 Z" fill="none" stroke="#4ade80" stroke-width="1.5" opacity="0.6"/>
        </svg>
        <div class="footer-links">
            <a href="https://github.com/ObviousSatire/GaiaAI">Source on GitHub</a>
            <a href="https://doi.org/10.5281/zenodo.22949286">Open datasets</a>
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
        const duration = 2000;
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
