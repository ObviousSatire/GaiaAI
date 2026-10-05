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
        <circle class="cell-pulse" cx="200" cy="150" r="80" fill="url(#cellGlow)"/>
        <circle class="cell-pulse" cx="1600" cy="700" r="120" fill="url(#cellGlow)"/>
        <circle class="cell-pulse" cx="1200" cy="200" r="60" fill="url(#cellGlow)"/>
        <g class="vine-sway" opacity="0.4">
            <path d="M100,900 Q150,700 80,500 Q140,300 100,100" stroke="#4ade80" stroke-width="1.5" fill="none"/>
        </g>
        <g class="vine-sway" opacity="0.35">
            <path d="M1700,900 Q1650,700 1720,500 Q1660,300 1700,100" stroke="#34d399" stroke-width="1.5" fill="none"/>
        </g>
        <g class="helix-flow" transform="translate(900, 450)">
            <path d="M-1200,0 Q-600,-220 0,0 T1200,0" stroke="url(#helixGrad)" stroke-width="1.8" fill="none"/>
            <path d="M-1200,0 Q-600,220 0,0 T1200,0" stroke="url(#helixGrad)" stroke-width="1.8" fill="none"/>
        </g>
        <g>
            <circle class="particle" cx="200" cy="200" r="3" fill="#4ade80"/>
            <circle class="particle" cx="500" cy="680" r="2.5" fill="#a7f3d0"/>
            <circle class="particle" cx="1400" cy="180" r="3" fill="#34d399"/>
            <circle class="particle" cx="1650" cy="580" r="2.5" fill="#60a5fa"/>
            <circle class="particle" cx="900" cy="100" r="3" fill="#4ade80"/>
            <circle class="particle" cx="300" cy="500" r="2.5" fill="#a7f3d0"/>
            <circle class="particle" cx="1500" cy="420" r="3" fill="#4ade80"/>
            <circle class="particle" cx="700" cy="780" r="2.5" fill="#60a5fa"/>
        </g>
            <text class="float-label" x="150" y="120" style="font-family: monospace; font-size: 11px; fill: #4ade80; opacity: 0.25;">ATCG</text>
        <text class="float-label" x="1450" y="180" style="font-family: monospace; font-size: 10px; fill: #60a5fa; opacity: 0.2;">exon</text>
        <text class="float-label" x="350" y="620" style="font-family: monospace; font-size: 10px; fill: #a7f3d0; opacity: 0.2;">intron</text>
        <text class="float-label" x="1250" y="720" style="font-family: monospace; font-size: 11px; fill: #34d399; opacity: 0.25;">GC 0.62</text>
        <text class="float-label" x="750" y="780" style="font-family: monospace; font-size: 10px; fill: #4ade80; opacity: 0.2;">D = 1.16</text>
        <text class="float-label" x="1050" y="140" style="font-family: monospace; font-size: 10px; fill: #60a5fa; opacity: 0.2;">chr6</text>
        <text class="float-label" x="550" y="200" style="font-family: monospace; font-size: 9px; fill: #a7f3d0; opacity: 0.2;">HLA-B</text>
        <text class="float-label" x="1600" y="500" style="font-family: monospace; font-size: 10px; fill: #34d399; opacity: 0.2;">variant</text>
        <text class="float-label" x="250" y="400" style="font-family: monospace; font-size: 9px; fill: #4ade80; opacity: 0.2;">fractal</text>
</svg>

    <div class="eq-layer" aria-hidden="true">
        <span class="eq small"  style="top: 8%;  left: 5%;">
            H <span class="op">=</span> <span class="op">−</span> Σ <span class="v">p</span><sub>i</sub> <span class="f">log</span><sub>2</sub> <span class="v">p</span><sub>i</sub>
        </span>
        <span class="eq med"    style="top: 15%; left: 72%;">
            D <span class="op">=</span> <span class="f">lim</span><sub>ε→0</sub> <span class="f">log</span> N(ε) <span class="op">/</span> <span class="f">log</span>(1/ε)
        </span>
        <span class="eq small"  style="top: 22%; left: 30%;">
            E <span class="op">~</span> c · n<sup><span class="v">H</span></sup>
        </span>
        <span class="eq"        style="top: 30%; left: 82%;">
            <span class="v">P</span>(c | x)
        </span>
        <span class="eq med"    style="top: 38%; left: 8%;">
            E <span class="op">=</span> 4ε[ (σ/r)<sup><span class="n">12</span></sup> <span class="op">−</span> (σ/r)<sup><span class="n">6</span></sup> ]
        </span>
        <span class="eq small"  style="top: 44%; left: 60%;">
            w<sub>t+1</sub> <span class="op">=</span> w<sub>t</sub> <span class="op">−</span> η ∇L(w<sub>t</sub>)
        </span>
        <span class="eq large"  style="top: 52%; left: 20%;">
            <span class="v">F</span><sub>1</sub> <span class="op">=</span> <span class="n">2</span> · P · R <span class="op">/</span> (P + R)
        </span>
        <span class="eq med"    style="top: 60%; left: 78%;">
            E <span class="op">=</span> <span class="n">332</span> · q<sub>i</sub> q<sub>j</sub> · e<sup>−κr</sup> <span class="op">/</span> r
        </span>
        <span class="eq small"  style="top: 68%; left: 4%;">
            χ<sub>i</sub> <span class="op">←</span> χ<sub>i</sub> <span class="op">+</span> η q<sub>i</sub> <span class="op">+</span> Σ γ<sub>ij</sub> q<sub>j</sub>
        </span>
        <span class="eq"        style="top: 76%; left: 55%;">
            ΔG <span class="op">=</span> ⟨G⟩<sub>bound</sub> <span class="op">−</span> ⟨G⟩<sub>free</sub>
        </span>
        <span class="eq small"  style="top: 84%; left: 28%;">
            λ ∈ [<span class="n">0</span>, <span class="n">1</span>]
        </span>
        <span class="eq med"    style="top: 90%; left: 74%;">
            ∂E/∂t <span class="op">→</span> <span class="n">0</span>
        </span>
        <span class="eq small"  style="top: 12%; left: 45%;">
            ∫ p(x) dx <span class="op">=</span> <span class="n">1</span>
        </span>
        <span class="eq"        style="top: 65%; left: 40%;">
            <span class="op">∇</span>·F <span class="op">=</span> <span class="n">0</span>
        </span>
        <span class="eq small"  style="top: 48%; left: 88%;">
            Σ<sub>i</sub> q<sub>i</sub> <span class="op">=</span> <span class="n">0</span>
        </span>
        <span class="eq med"    style="top: 3%; left: 55%;">
            ⟨S⟩ <span class="op">=</span> <span class="op">−</span>k<sub>B</sub> Σ p<sub>i</sub> ln p<sub>i</sub>
        </span>
    </div>

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
                <div class="num static">1.08B</div>
                <div class="label">Variants mapped</div>
            </div>
            <div class="stat">
                <div class="num" data-count="25000000" data-format="m">0</div>
                <div class="label">Compounds indexed</div>
            </div>
            <div class="stat">
                <div class="num" data-count="500" data-format="plus">0</div>
                <div class="label">Curated sources</div>
            </div>
            <div class="stat">
                <div class="num" data-count="1" data-format="tb">0</div>
                <div class="label">Knowledge base</div>
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
            A system that reads the genome and reads the web. It discovers
            patterns, grows a knowledge graph, and improves continuously as
            new data arrives — from files, from databases, and from hundreds
            of curated reputable sources.
        </p>
        <p style="color: var(--fg-dim); font-size: 1.05rem; line-height: 1.8;">
            Most drug discovery starts with a hypothesis and tests it. GAIA
            starts with the raw genome and the raw literature, and works
            backward. Nothing is hand-coded. The system discovers its own
            patterns.
        </p>
    </div>
</section>

<section id="learning">
    <div class="container">
        <h2>How it <span class="accent">learns</span></h2>
        <p class="lead">
            Three loops, running continuously. Each one improves the system
            without anyone telling it what to look for.
        </p>

        <div class="learn-grid">
            <div class="learn-card">
                <div class="badge">01</div>
                <div class="icon-box">
                    <svg width="30" height="30" viewBox="0 0 40 40">
                        <circle cx="20" cy="20" r="14" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <path d="M8,20 Q20,12 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <path d="M8,20 Q20,28 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <circle cx="20" cy="20" r="2.5" fill="#a7f3d0"/>
                    </svg>
                </div>
                <svg class="inner-anim" viewBox="0 0 300 90" preserveAspectRatio="none">
                    <line x1="0" y1="45" x2="300" y2="45" stroke="#1c3628" stroke-width="0.5"/>
                    <path class="scan-wave" d="M0,45 Q15,15 30,45 T60,45 T90,45 T120,45 T150,45 T180,45 T210,45 T240,45 T270,45 T300,45" stroke="#4ade80" stroke-width="1.8" fill="none"/>
                    <path class="scan-wave" d="M0,45 Q15,75 30,45 T60,45 T90,45 T120,45 T150,45 T180,45 T210,45 T240,45 T270,45 T300,45" stroke="#a7f3d0" stroke-width="1" fill="none" opacity="0.5" style="animation-delay: -2.5s"/>
                    <circle cx="40" cy="45" r="2" fill="#4ade80"/>
                    <circle cx="120" cy="45" r="2" fill="#60a5fa"/>
                    <circle cx="200" cy="45" r="2" fill="#34d399"/>
                    <circle cx="260" cy="45" r="2" fill="#a7f3d0"/>
                </svg>

                <h3>Discovering patterns</h3>
                <p>Raw sequence in. The system finds its own structure — coding regions, conserved blocks, regulatory signals — without being told what to look for.</p>
                <ul class="step-list">
                    <li><span class="bullet"></span><div><strong>Ingest</strong> <span>— full chromosomes with curated labels</span></div></li>
                    <li><span class="bullet"></span><div><strong>Extract</strong> <span>— entropy, GC, motif, conservation</span></div></li>
                    <li><span class="bullet"></span><div><strong>Train</strong> <span>— classifier updates by gradient descent</span></div></li>
                    <li><span class="bullet"></span><div><strong>Validate</strong> <span>— cross-chromosome and cross-species</span></div></li>
                </ul>
            </div>

            <div class="learn-card">
                <div class="badge">02</div>
                <div class="icon-box">
                    <svg width="30" height="30" viewBox="0 0 40 40">
                        <circle cx="9" cy="20" r="3" fill="#60a5fa"/>
                        <circle cx="20" cy="9" r="3" fill="#60a5fa"/>
                        <circle cx="31" cy="20" r="3" fill="#60a5fa"/>
                        <circle cx="20" cy="31" r="3" fill="#60a5fa"/>
                        <line x1="9" y1="20" x2="20" y2="9" stroke="#60a5fa" stroke-width="1"/>
                        <line x1="20" y1="9" x2="31" y2="20" stroke="#60a5fa" stroke-width="1"/>
                        <line x1="31" y1="20" x2="20" y2="31" stroke="#60a5fa" stroke-width="1"/>
                        <line x1="20" y1="31" x2="9" y2="20" stroke="#60a5fa" stroke-width="1"/>
                    </svg>
                </div>
                <svg class="inner-anim" viewBox="0 0 300 90" preserveAspectRatio="none">
                    <line class="grow-edge" x1="60" y1="45" x2="120" y2="20" stroke="#60a5fa" stroke-width="1.2"/>
                    <line class="grow-edge e2" x1="60" y1="45" x2="120" y2="70" stroke="#60a5fa" stroke-width="1.2"/>
                    <line class="grow-edge e3" x1="120" y1="20" x2="180" y2="45" stroke="#a7f3d0" stroke-width="1.2"/>
                    <line class="grow-edge e4" x1="120" y1="70" x2="180" y2="45" stroke="#a7f3d0" stroke-width="1.2"/>
                    <line class="grow-edge e5" x1="180" y1="45" x2="240" y2="45" stroke="#4ade80" stroke-width="1.5"/>
                    <circle class="grow-node" cx="60" cy="45" r="6" fill="#4ade80"/>
                    <circle class="grow-node g2" cx="120" cy="20" r="5" fill="#60a5fa"/>
                    <circle class="grow-node g3" cx="120" cy="70" r="5" fill="#34d399"/>
                    <circle class="grow-node g4" cx="180" cy="45" r="6" fill="#a7f3d0"/>
                    <circle class="grow-node g5" cx="240" cy="45" r="7" fill="#4ade80"/>
                </svg>

                <h3>Growing the graph</h3>
                <p>Every new finding connects. Variants, genes, pathways, diseases, compounds — each relation adds to a network that grows with the field.</p>
                <ul class="step-list">
                    <li><span class="bullet"></span><div><strong>Ingest</strong> <span>— mappings, bindings, structures</span></div></li>
                    <li><span class="bullet"></span><div><strong>Connect</strong> <span>— variant → gene → disease → compound</span></div></li>
                    <li><span class="bullet"></span><div><strong>Query</strong> <span>— score candidates, rank outcomes</span></div></li>
                    <li><span class="bullet"></span><div><strong>Retrain</strong> <span>— new pairs improve predictions</span></div></li>
                </ul>
            </div>

            <div class="learn-card">
                <div class="badge">03</div>
                <div class="icon-box">
                    <svg width="30" height="30" viewBox="0 0 40 40">
                        <path d="M8,20 A12,12 0 0,1 32,20" fill="none" stroke="#a7f3d0" stroke-width="1.5"/>
                        <path d="M32,20 A12,12 0 0,1 8,20" fill="none" stroke="#a7f3d0" stroke-width="1.5"/>
                        <polygon points="30,14 32,20 26,20" fill="#a7f3d0"/>
                        <polygon points="10,26 8,20 14,20" fill="#a7f3d0"/>
                    </svg>
                </div>
                <svg class="inner-anim" viewBox="0 0 300 90" preserveAspectRatio="none">
                    <circle cx="60" cy="45" r="28" fill="none" stroke="#1c3628" stroke-width="1.5"/>
                    <circle cx="60" cy="45" r="28" fill="none" stroke="#4ade80" stroke-width="1.5" stroke-dasharray="44 176" stroke-linecap="round">
                        <animateTransform attributeName="transform" type="rotate" from="0 60 45" to="360 60 45" dur="3s" repeatCount="indefinite"/>
                    </circle>
                    <text x="60" y="49" text-anchor="middle" font-size="9" fill="#a7f3d0" font-family="monospace">loop</text>

                    <line x1="100" y1="45" x2="140" y2="45" stroke="#34d399" stroke-width="1" stroke-dasharray="4 4"/>
                    <polygon points="140,42 148,45 140,48" fill="#34d399"/>

                    <circle cx="180" cy="45" r="18" fill="none" stroke="#60a5fa" stroke-width="1.5" stroke-dasharray="30 84" stroke-linecap="round">
                        <animateTransform attributeName="transform" type="rotate" from="360 180 45" to="0 180 45" dur="2.5s" repeatCount="indefinite"/>
                    </circle>
                    <text x="180" y="49" text-anchor="middle" font-size="9" fill="#a7f3d0" font-family="monospace">refit</text>

                    <line x1="210" y1="45" x2="240" y2="45" stroke="#34d399" stroke-width="1" stroke-dasharray="4 4"/>
                    <polygon points="240,42 248,45 240,48" fill="#34d399"/>

                    <circle cx="265" cy="45" r="14" fill="none" stroke="#a7f3d0" stroke-width="1.5" stroke-dasharray="22 66" stroke-linecap="round">
                        <animateTransform attributeName="transform" type="rotate" from="0 265 45" to="360 265 45" dur="2s" repeatCount="indefinite"/>
                    </circle>
                    <text x="265" y="49" text-anchor="middle" font-size="9" fill="#a7f3d0" font-family="monospace">+ev</text>
                </svg>

                <h3>Continuous loop</h3>
                <p>The system improves on its own. New data arrives, models retrain, and if it helps — prediction improves. If not, it fades.</p>
                <ul class="step-list">
                    <li><span class="bullet"></span><div><strong>New evidence</strong> <span>— variant, paper, structure</span></div></li>
                    <li><span class="bullet"></span><div><strong>Context fetched</strong> <span>— class, conservation, motif</span></div></li>
                    <li><span class="bullet"></span><div><strong>Model retrains</strong> <span>— weights adjust on new inputs</span></div></li>
                    <li><span class="bullet"></span><div><strong>Impact measured</strong> <span>— help stays, noise fades</span></div></li>
                </ul>
            </div>
        </div>
    </div>
</section>

<section id="evidence">
    <div class="container">
        <h2>Evidence across <span class="accent">every layer</span></h2>
        <p class="lead">
            Predictions are checked against three independent kinds of
            evidence — computational, cellular, and physiological. A claim
            that survives all three is worth acting on.
        </p>

        <div class="evidence-grid">
            <div class="evidence-card">
                <span class="tag">In silico</span>
                <h3>Computational</h3>
                <p>Before anything touches a cell, every prediction is stress-tested in pure computation. Models run, scores are produced, and confidence is estimated from the spread of agreement across independent methods.</p>
                <ul>
                    <li><strong>Structure prediction</strong> — check every candidate against modeled protein geometry</li>
                    <li><strong>Binding simulation</strong> — estimate interaction strength across methods</li>
                    <li><strong>Cross-validation</strong> — hold out data the model never saw</li>
                    <li><strong>Confidence intervals</strong> — measure agreement across independent approaches</li>
                </ul>
            </div>

            <div class="evidence-card">
                <span class="tag">In vitro</span>
                <h3>Cellular</h3>
                <p>Predictions are compared against real cell-based assays from public literature. Pathway activity, gene expression, and compound cytotoxicity all feed back into the model.</p>
                <ul>
                    <li><strong>Cell-line assays</strong> — activity against published screens</li>
                    <li><strong>Pathway response</strong> — how signaling shifts under treatment</li>
                    <li><strong>Gene expression</strong> — transcript-level confirmation of predicted effects</li>
                    <li><strong>Cytotoxicity profiles</strong> — safe dose ranges from established tests</li>
                </ul>
            </div>

            <div class="evidence-card">
                <span class="tag">In vivo</span>
                <h3>Physiological</h3>
                <p>Protocols are evaluated against animal model studies and human trial data. Where the model predicts a specific outcome, that outcome is checked against real physiological responses in published cohorts.</p>
                <ul>
                    <li><strong>Animal disease models</strong> — response in established model systems</li>
                    <li><strong>Clinical trial data</strong> — dosing, outcomes, adverse events</li>
                    <li><strong>Human cohorts</strong> — time-to-response across published studies</li>
                    <li><strong>Longitudinal outcomes</strong> — durability of effect at follow-up</li>
                </ul>
            </div>
        </div>

        <div class="evidence-cross">
            <h3>Cross-cutting validation</h3>
            <div class="cross-grid">
                <div class="cross-item">
                    <div class="cross-icon">
                        <svg width="28" height="28" viewBox="0 0 40 40">
                            <circle cx="20" cy="20" r="14" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                            <path d="M8,20 Q20,12 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                            <path d="M8,20 Q20,28 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        </svg>
                    </div>
                    <div>
                        <div class="cross-title">Cross-species</div>
                        <div class="cross-desc">Patterns that hold across evolutionary distance are more likely to reflect real biology.</div>
                    </div>
                </div>

                <div class="cross-item">
                    <div class="cross-icon">
                        <svg width="28" height="28" viewBox="0 0 40 40">
                            <circle cx="14" cy="18" r="6" fill="none" stroke="#60a5fa" stroke-width="1.5"/>
                            <circle cx="26" cy="18" r="6" fill="none" stroke="#60a5fa" stroke-width="1.5"/>
                            <circle cx="20" cy="30" r="6" fill="none" stroke="#60a5fa" stroke-width="1.5"/>
                        </svg>
                    </div>
                    <div>
                        <div class="cross-title">Animal models</div>
                        <div class="cross-desc">Predictions checked against real physiological responses in established model systems.</div>
                    </div>
                </div>

                <div class="cross-item">
                    <div class="cross-icon">
                        <svg width="28" height="28" viewBox="0 0 40 40">
                            <rect x="8" y="10" width="24" height="20" rx="3" fill="none" stroke="#a7f3d0" stroke-width="1.5"/>
                            <line x1="16" y1="20" x2="24" y2="20" stroke="#a7f3d0" stroke-width="1.5"/>
                            <line x1="20" y1="16" x2="20" y2="24" stroke="#a7f3d0" stroke-width="1.5"/>
                        </svg>
                    </div>
                    <div>
                        <div class="cross-title">Human trial models</div>
                        <div class="cross-desc">Protocols evaluated against clinical data — dosing, outcomes, adverse events, timing.</div>
                    </div>
                </div>

                <div class="cross-item">
                    <div class="cross-icon">
                        <svg width="28" height="28" viewBox="0 0 40 40">
                            <path d="M6,32 L6,24 L12,24 L12,18 L18,18 L18,26 L24,26 L24,14 L30,14 L30,10 L34,10" fill="none" stroke="#34d399" stroke-width="2" stroke-linejoin="round"/>
                        </svg>
                    </div>
                    <div>
                        <div class="cross-title">Held-out evaluation</div>
                        <div class="cross-desc">Tested on chromosomes, diseases, and compounds never seen during training.</div>
                    </div>
                </div>
            </div>
        </div>

        <div class="outputs-strip">
            <div class="output-item">
                <svg width="32" height="32" viewBox="0 0 32 32">
                    <circle cx="16" cy="16" r="12" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="16" cy="16" r="6" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="16" cy="16" r="2.5" fill="#a7f3d0"/>
                </svg>
                <div class="name">Ranked candidates</div>
                <div class="sub">Compounds ordered by evidence</div>
            </div>
            <div class="output-item">
                <svg width="32" height="32" viewBox="0 0 32 32">
                    <path d="M4,24 L4,16 L10,16 L10,10 L16,10 L16,18 L22,18 L22,6 L28,6" fill="none" stroke="#60a5fa" stroke-width="2" stroke-linejoin="round"/>
                </svg>
                <div class="name">Protocol timeline</div>
                <div class="sub">Outcomes across time</div>
            </div>
            <div class="output-item">
                <svg width="32" height="32" viewBox="0 0 32 32">
                    <rect x="6" y="6" width="20" height="20" rx="3" fill="none" stroke="#a7f3d0" stroke-width="1.5"/>
                    <line x1="11" y1="12" x2="21" y2="12" stroke="#a7f3d0" stroke-width="1.5"/>
                    <line x1="11" y1="16" x2="21" y2="16" stroke="#a7f3d0" stroke-width="1.5"/>
                    <line x1="11" y1="20" x2="17" y2="20" stroke="#a7f3d0" stroke-width="1.5"/>
                </svg>
                <div class="name">Evidence report</div>
                <div class="sub">Full trace from signal to plan</div>
            </div>
            <div class="output-item">
                <svg width="32" height="32" viewBox="0 0 32 32">
                    <path d="M16,4 L28,10 L28,22 L16,28 L4,22 L4,10 Z" fill="none" stroke="#34d399" stroke-width="1.5"/>
                    <circle cx="16" cy="16" r="3" fill="#34d399"/>
                </svg>
                <div class="name">Confidence score</div>
                <div class="sub">How much evidence supports it</div>
            </div>
        </div>
    </div>
</section>

<section id="sources">
    <div class="container">
        <h2>It reads the <span class="accent">open web</span></h2>
        <p class="lead">
            The system doesn't wait for someone to hand it data. It reads
            hundreds of curated, reputable URLs — peer-reviewed literature,
            reference genomes, protein structures, clinical registries — and
            grows as new findings are published.
        </p>

        <div class="web-layout">
            <div class="web-visual">
                <svg viewBox="0 0 400 400" preserveAspectRatio="xMidYMid meet">
                    <defs>
                        <radialGradient id="hubGrad" cx="50%" cy="50%" r="50%">
                            <stop offset="0%" stop-color="#a7f3d0" stop-opacity="1"/>
                            <stop offset="60%" stop-color="#4ade80" stop-opacity="0.5"/>
                            <stop offset="100%" stop-color="#4ade80" stop-opacity="0"/>
                        </radialGradient>
                    </defs>

                    <g class="spin-1">
                        <ellipse cx="200" cy="200" rx="150" ry="60" fill="none" stroke="#4ade80" stroke-width="0.5" opacity="0.35" transform="rotate(20 200 200)"/>
                    </g>
                    <g class="spin-2">
                        <ellipse cx="200" cy="200" rx="175" ry="70" fill="none" stroke="#60a5fa" stroke-width="0.5" opacity="0.25" transform="rotate(-30 200 200)"/>
                    </g>

                    <circle class="ring-out" cx="200" cy="200" r="40" fill="none" stroke="#4ade80" stroke-width="1.2"/>
                    <circle class="ring-out r2" cx="200" cy="200" r="40" fill="none" stroke="#4ade80" stroke-width="1.2"/>
                    <circle class="ring-out r3" cx="200" cy="200" r="40" fill="none" stroke="#4ade80" stroke-width="1.2"/>

                    <line class="flow" x1="200" y1="200" x2="70" y2="70" stroke="#60a5fa" stroke-width="1.6"/>
                    <line class="flow f2" x1="200" y1="200" x2="330" y2="70" stroke="#a7f3d0" stroke-width="1.6"/>
                    <line class="flow f3" x1="200" y1="200" x2="70" y2="330" stroke="#34d399" stroke-width="1.6"/>
                    <line class="flow f4" x1="200" y1="200" x2="330" y2="330" stroke="#4ade80" stroke-width="1.6"/>
                    <line class="flow f5" x1="200" y1="200" x2="200" y2="45" stroke="#60a5fa" stroke-width="1.2"/>
                    <line class="flow f6" x1="200" y1="200" x2="200" y2="355" stroke="#34d399" stroke-width="1.2"/>
                    <line class="flow f7" x1="200" y1="200" x2="45" y2="200" stroke="#a7f3d0" stroke-width="1.2"/>
                    <line class="flow f8" x1="200" y1="200" x2="355" y2="200" stroke="#4ade80" stroke-width="1.2"/>

                    <g class="center-pulse">
                        <circle cx="200" cy="200" r="58" fill="url(#hubGrad)" opacity="0.45"/>
                        <circle cx="200" cy="200" r="36" fill="none" stroke="#a7f3d0" stroke-width="2"/>
                        <text x="200" y="206" text-anchor="middle" font-family="monospace" font-size="14" fill="#a7f3d0" font-weight="bold">GAIA</text>
                    </g>

                    <circle class="blink" cx="70" cy="70" r="7" fill="#60a5fa"/>
                    <text x="70" y="46" text-anchor="middle" font-size="10" fill="#8fa89c" font-family="system-ui">Literature</text>

                    <circle class="blink b2" cx="330" cy="70" r="7" fill="#a7f3d0"/>
                    <text x="330" y="46" text-anchor="middle" font-size="10" fill="#8fa89c" font-family="system-ui">Genomes</text>

                    <circle class="blink b3" cx="70" cy="330" r="7" fill="#34d399"/>
                    <text x="70" y="360" text-anchor="middle" font-size="10" fill="#8fa89c" font-family="system-ui">Proteins</text>

                    <circle class="blink b4" cx="330" cy="330" r="7" fill="#4ade80"/>
                    <text x="330" y="360" text-anchor="middle" font-size="10" fill="#8fa89c" font-family="system-ui">Variants</text>

                    <circle class="blink b5" cx="200" cy="45" r="6" fill="#60a5fa"/>
                    <text x="200" y="26" text-anchor="middle" font-size="9" fill="#8fa89c" font-family="system-ui">Pathways</text>

                    <circle class="blink b6" cx="200" cy="355" r="6" fill="#34d399"/>
                    <text x="200" y="384" text-anchor="middle" font-size="9" fill="#8fa89c" font-family="system-ui">Compounds</text>

                    <circle class="blink b7" cx="45" cy="200" r="6" fill="#a7f3d0"/>
                    <text x="30" y="180" text-anchor="middle" font-size="9" fill="#8fa89c" font-family="system-ui">Trials</text>

                    <circle class="blink b8" cx="355" cy="200" r="6" fill="#4ade80"/>
                    <text x="372" y="180" text-anchor="middle" font-size="9" fill="#8fa89c" font-family="system-ui">Structures</text>
                </svg>
            </div>

            <div class="web-info">
                <span class="web-tag"><span class="live-dot"></span> Hundreds of curated sources</span>
                <h3>Reputable <span class="accent">URLs</span>, continuously read</h3>
                <p>
                    Peer-reviewed publications, national reference databases,
                    protein structure archives, clinical trial registries.
                    Each source is vetted. Each new finding updates the graph.
                </p>

                <div class="web-chips">
                    <div class="web-chip">
                        <div class="chip-title">Publications</div>
                        <div class="chip-desc">Peer-reviewed findings</div>
                    </div>
                    <div class="web-chip">
                        <div class="chip-title">Genomes</div>
                        <div class="chip-desc">Reference assemblies</div>
                    </div>
                    <div class="web-chip">
                        <div class="chip-title">Proteins</div>
                        <div class="chip-desc">Structures and functions</div>
                    </div>
                    <div class="web-chip">
                        <div class="chip-title">Variants</div>
                        <div class="chip-desc">Population and clinical</div>
                    </div>
                    <div class="web-chip">
                        <div class="chip-title">Compounds</div>
                        <div class="chip-desc">Bioactivity and libraries</div>
                    </div>
                    <div class="web-chip">
                        <div class="chip-title">Trials</div>
                        <div class="chip-desc">Clinical registries</div>
                    </div>
                </div>
            </div>
        </div>

        <div class="reading-ticker">
            <div class="ticker-track">
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Peer-reviewed literature</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Reference genomes</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Protein structure archives</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Population variant databases</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Clinical trial registries</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Bioactivity datasets</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Pathway databases</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Disease association catalogs</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Compound libraries</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Structural archives</span>
                <!-- duplicate for seamless loop -->
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Peer-reviewed literature</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Reference genomes</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Protein structure archives</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Population variant databases</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Clinical trial registries</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Bioactivity datasets</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Pathway databases</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Disease association catalogs</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Compound libraries</span>
                <span class="ticker-item"><span class="dot"></span><span class="label">reading</span>Structural archives</span>
            </div>
        </div>

        <div class="scan-flow-wrap">
            <h3>The continuous loop</h3>
            <div class="scan-row">
                <div class="scan-box">
                    <span class="icon">🌐</span>
                    <div class="label">Crawl</div>
                    <div class="sub">Curated URLs</div>
                </div>
                <div class="scan-box">
                    <span class="icon">📖</span>
                    <div class="label">Parse</div>
                    <div class="sub">Extract relations</div>
                </div>
                <div class="scan-box">
                    <span class="icon">✓</span>
                    <div class="label">Validate</div>
                    <div class="sub">Cross-check sources</div>
                </div>
                <div class="scan-box">
                    <span class="icon">🌱</span>
                    <div class="label">Integrate</div>
                    <div class="sub">Grow the graph</div>
                </div>
                <div class="scan-box">
                    <span class="icon">📈</span>
                    <div class="label">Retrain</div>
                    <div class="sub">Learn from new data</div>
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
                </svg>
                <h3>Map the variants</h3>
                <p>Population variation placed in context. Every variant associated with its gene, pathway, and evidence.</p>
            </div>
            <div class="stage">
                <div class="stage-num">STAGE 03</div>
                <svg width="44" height="44" viewBox="0 0 40 40">
                    <rect x="8" y="12" width="24" height="16" rx="3" fill="none" stroke="#a7f3d0" stroke-width="1.5"/>
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
            </div>

            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <rect x="4" y="14" width="9" height="9" rx="1.5" fill="#34d399"/>
                    <rect x="15" y="14" width="9" height="9" rx="1.5" fill="#34d399" opacity="0.7"/>
                    <rect x="26" y="14" width="9" height="9" rx="1.5" fill="#34d399" opacity="0.5"/>
                </svg>
                <h3>Compound libraries</h3>
                <p>Multiple curated libraries of small molecules and natural products. Thousands upon thousands of candidates ready to be screened against any target.</p>
            </div>

            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <circle cx="20" cy="20" r="14" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="20" cy="20" r="7" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <circle cx="20" cy="20" r="2.5" fill="#4ade80"/>
                </svg>
                <h3>Interaction scoring</h3>
                <p>Multiple scoring approaches combined into one ranking. Physical, chemical, and contextual evidence rolled into a single number.</p>
            </div>

            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <path d="M6,32 L6,24 L14,24 L14,16 L22,16 L22,24 L30,24 L30,10 L34,10" fill="none" stroke="#60a5fa" stroke-width="2" stroke-linejoin="round"/>
                </svg>
                <h3>Protocol design</h3>
                <p>Simulated multi-compound protocols across time. Predicted outcomes, risks, and safety margins — all in one plan.</p>
            </div>

            <div class="capability">
                <svg class="glyph" width="44" height="44" viewBox="0 0 40 40">
                    <path d="M6,12 L6,28 M12,12 L12,28 M18,12 L18,28 M24,12 L24,28 M30,12 L30,28 M36,12 L36,28" stroke="#a7f3d0" stroke-width="1.5"/>
                </svg>
                <h3>Link prediction</h3>
                <p>A trained classifier that predicts missing links in the graph. Improves automatically as the graph grows.</p>
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

<section class="use-it">
    <div class="container">
        <h2>Use it</h2>
        <p class="lead">Three ways to start — depending on what you want to build on.</p>

        <div class="use-grid">
            <a class="use-card" href="https://doi.org/10.5281/zenodo.22949286" target="_blank" rel="noopener">
                <svg width="32" height="32" viewBox="0 0 40 40">
                    <ellipse cx="20" cy="12" rx="12" ry="4" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                    <path d="M8,12 L8,28 Q8,32 20,32 Q32,32 32,28 L32,12" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                </svg>
                <div class="title">Explore the datasets</div>
                <div class="desc">Every stage of the pipeline, archived with permanent identifiers. Downloads, sizes, and contents for each dataset.</div>
                <div class="arrow">Open datasets →</div>
            </a>

            <a class="use-card" href="https://github.com/ObviousSatire/GaiaAI" target="_blank" rel="noopener">
                <svg width="32" height="32" viewBox="0 0 40 40">
                    <path d="M14,6 L6,20 L14,34" fill="none" stroke="#60a5fa" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    <path d="M26,6 L34,20 L26,34" fill="none" stroke="#60a5fa" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    <line x1="22" y1="10" x2="18" y2="30" stroke="#60a5fa" stroke-width="2" stroke-linecap="round"/>
                </svg>
                <div class="title">Read the source</div>
                <div class="desc">C++17 and Python stdlib only. No external dependencies. The physics engine, the learning pipeline, and the scanning loop.</div>
                <div class="arrow">Open source →</div>
            </a>

            <a class="use-card" href="#pipeline" target="_self">
                <svg width="32" height="32" viewBox="0 0 40 40">
                    <path d="M6,32 L6,24 L14,24 L14,16 L22,16 L22,26 L30,26 L30,12 L34,12" fill="none" stroke="#a7f3d0" stroke-width="2" stroke-linejoin="round"/>
                </svg>
                <div class="title">Follow the pipeline</div>
                <div class="desc">See how raw genome input becomes a treatment protocol — the five stages, the three evidence layers, and the outputs.</div>
                <div class="arrow">Jump to pipeline →</div>
            </a>
        </div>
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
            <a href="#learning">How it learns</a>
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
        const duration = 2000;
        const start = performance.now();
        function update(now) {
            const t = Math.min(1, (now - start) / duration);
            const ease = 1 - Math.pow(1 - t, 3);
            const val = Math.floor(target * ease);
            if (fmt === 'k' && val >= 1000) {
                el.textContent = (val / 1000).toFixed(2).replace(/\.00$/, '') + 'M';
            } else if (fmt === 'b') {
                el.textContent = val + 'B+';
            } else if (fmt === 'm' && val >= 1000000) {
                el.textContent = (val / 1000000).toFixed(0) + 'M+';
            } else if (fmt === 'plus') {
                el.textContent = val + '+';
            } else if (fmt === 'tb') {
                el.textContent = val + ' TB+';
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
</script>

</body>
</html>
