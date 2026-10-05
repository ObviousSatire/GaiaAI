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
            backward. Nothing is hand-coded. Both layers discover their own
            patterns.
        </p>
    </div>
</section>

<section id="learning">
    <div class="container">
        <div class="learn-center">
            <h2>How it <span class="accent">learns</span></h2>
            <p class="lead">
                Nothing is hand-coded. The system reads raw signal, discovers
                its own features, and updates as new evidence arrives.
            </p>
        </div>

        <div class="learn-flow">
            <div class="learn-block">
                <div class="num-badge">01</div>
                <div class="stage-icon">
                    <svg width="36" height="36" viewBox="0 0 40 40">
                        <circle cx="20" cy="20" r="14" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <path d="M8,20 Q20,12 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <path d="M8,20 Q20,28 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <circle cx="20" cy="20" r="2.5" fill="#a7f3d0"/>
                    </svg>
                </div>
                <h3>Discovering patterns</h3>
                <p>Raw sequence in. The system finds its own structure — coding regions, conserved blocks, regulatory signals — without being told what to look for.</p>
                <div class="steps">
                    <div class="mini-step"><span class="dot"></span><div><strong>Ingest</strong> <span>— full chromosomes with curated labels</span></div></div>
                    <div class="mini-step"><span class="dot"></span><div><strong>Extract</strong> <span>— entropy, GC, motif, conservation</span></div></div>
                    <div class="mini-step"><span class="dot"></span><div><strong>Train</strong> <span>— classifier updates by gradient descent</span></div></div>
                    <div class="mini-step"><span class="dot"></span><div><strong>Validate</strong> <span>— cross-chromosome and cross-species</span></div></div>
                </div>
            </div>

            <div class="learn-block">
                <div class="num-badge">02</div>
                <div class="stage-icon">
                    <svg width="36" height="36" viewBox="0 0 40 40">
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
                <h3>Growing the graph</h3>
                <p>Every new finding connects. Variants, genes, pathways, diseases, compounds — each relation adds to a network that grows with the field.</p>
                <div class="steps">
                    <div class="mini-step"><span class="dot"></span><div><strong>Ingest</strong> <span>— mappings, bindings, structures</span></div></div>
                    <div class="mini-step"><span class="dot"></span><div><strong>Connect</strong> <span>— variant → gene → disease → compound</span></div></div>
                    <div class="mini-step"><span class="dot"></span><div><strong>Query</strong> <span>— score candidates, rank outcomes</span></div></div>
                    <div class="mini-step"><span class="dot"></span><div><strong>Retrain</strong> <span>— new pairs improve predictions</span></div></div>
                </div>
            </div>

            <div class="learn-block">
                <div class="num-badge">03</div>
                <div class="stage-icon">
                    <svg width="36" height="36" viewBox="0 0 40 40">
                        <path d="M8,20 A12,12 0 0,1 32,20" fill="none" stroke="#a7f3d0" stroke-width="1.5"/>
                        <path d="M32,20 A12,12 0 0,1 8,20" fill="none" stroke="#a7f3d0" stroke-width="1.5"/>
                        <polygon points="30,14 32,20 26,20" fill="#a7f3d0"/>
                        <polygon points="10,26 8,20 14,20" fill="#a7f3d0"/>
                    </svg>
                </div>
                <h3>Continuous loop</h3>
                <p>The system improves on its own. New data arrives, models retrain, and if it helps — prediction improves. If not, it fades.</p>
                <div class="steps">
                    <div class="mini-step"><span class="dot"></span><div><strong>New evidence</strong> <span>— variant, paper, structure</span></div></div>
                    <div class="mini-step"><span class="dot"></span><div><strong>Context fetched</strong> <span>— class, conservation, motif</span></div></div>
                    <div class="mini-step"><span class="dot"></span><div><strong>Model retrains</strong> <span>— weights adjust on new inputs</span></div></div>
                    <div class="mini-step"><span class="dot"></span><div><strong>Impact measured</strong> <span>— help stays, noise fades</span></div></div>
                </div>
            </div>
        </div>
    </div>
</section>
<section id="sources">
    <div class="container">
        <h2>It reads the <span class="accent">open web</span></h2>
        <p class="lead">
            The system doesn't wait for someone to hand it data. It crawls
            hundreds of curated, reputable URLs — peer-reviewed literature,
            reference genomes, protein structures, clinical registries — and
            grows as new findings are published.
        </p>

        <div class="web-hero">
            <div class="web-content">
                <div class="web-graphic">
                    <svg viewBox="0 0 400 440" preserveAspectRatio="xMidYMid meet">
                        <defs>
                            <radialGradient id="hubCore" cx="50%" cy="50%" r="50%">
                                <stop offset="0%" stop-color="#a7f3d0" stop-opacity="1"/>
                                <stop offset="60%" stop-color="#4ade80" stop-opacity="0.6"/>
                                <stop offset="100%" stop-color="#4ade80" stop-opacity="0"/>
                            </radialGradient>
                        </defs>

                        <!-- Rotating orbital rings -->
                        <g class="rot-a"><ellipse cx="200" cy="220" rx="150" ry="65" fill="none" stroke="#4ade80" stroke-width="0.6" opacity="0.35" transform="rotate(20 200 220)"/></g>
                        <g class="rot-b"><ellipse cx="200" cy="220" rx="175" ry="72" fill="none" stroke="#60a5fa" stroke-width="0.5" opacity="0.25" transform="rotate(-25 200 220)"/></g>
                        <g class="rot-c"><ellipse cx="200" cy="220" rx="130" ry="55" fill="none" stroke="#a7f3d0" stroke-width="0.6" opacity="0.3" transform="rotate(55 200 220)"/></g>

                        <!-- Expanding pulse rings -->
                        <circle class="pulse-ring" cx="200" cy="220" r="40" fill="none" stroke="#4ade80" stroke-width="1.2"/>
                        <circle class="pulse-ring" cx="200" cy="220" r="40" fill="none" stroke="#4ade80" stroke-width="1.2"/>
                        <circle class="pulse-ring" cx="200" cy="220" r="40" fill="none" stroke="#4ade80" stroke-width="1.2"/>

                        <!-- Links with flowing dashes -->
                        <line class="link d1" x1="200" y1="220" x2="70" y2="80" stroke="#60a5fa" stroke-width="1.6"/>
                        <line class="link d2" x1="200" y1="220" x2="330" y2="80" stroke="#a7f3d0" stroke-width="1.6"/>
                        <line class="link d3" x1="200" y1="220" x2="70" y2="360" stroke="#34d399" stroke-width="1.6"/>
                        <line class="link d4" x1="200" y1="220" x2="330" y2="360" stroke="#4ade80" stroke-width="1.6"/>
                        <line class="link d5" x1="200" y1="220" x2="200" y2="55" stroke="#60a5fa" stroke-width="1.2"/>
                        <line class="link d6" x1="200" y1="220" x2="200" y2="395" stroke="#34d399" stroke-width="1.2"/>
                        <line class="link d7" x1="200" y1="220" x2="55" y2="220" stroke="#a7f3d0" stroke-width="1.2"/>
                        <line class="link d8" x1="200" y1="220" x2="345" y2="220" stroke="#4ade80" stroke-width="1.2"/>

                        <!-- Central hub -->
                        <g class="hub">
                            <circle cx="200" cy="220" r="65" fill="url(#hubCore)" opacity="0.5"/>
                            <circle cx="200" cy="220" r="40" fill="none" stroke="#a7f3d0" stroke-width="2.5"/>
                            <circle cx="200" cy="220" r="48" fill="none" stroke="#4ade80" stroke-width="0.6" opacity="0.6"/>
                            <text x="200" y="226" text-anchor="middle" font-family="monospace" font-size="15" fill="#a7f3d0" font-weight="bold">GAIA</text>
                        </g>

                        <!-- Source nodes -->
                        <g>
                            <circle class="n-halo h1" cx="70" cy="80" r="14" fill="none" stroke="#60a5fa" stroke-width="0.8"/>
                            <circle class="n n1" cx="70" cy="80" r="7" fill="#60a5fa"/>
                            <text class="lbl l1" x="70" y="52" text-anchor="middle" font-size="10" fill="#8fa89c" font-family="system-ui">Literature</text>
                        </g>
                        <g>
                            <circle class="n-halo h2" cx="330" cy="80" r="14" fill="none" stroke="#a7f3d0" stroke-width="0.8"/>
                            <circle class="n n2" cx="330" cy="80" r="7" fill="#a7f3d0"/>
                            <text class="lbl l2" x="330" y="52" text-anchor="middle" font-size="10" fill="#8fa89c" font-family="system-ui">Genomes</text>
                        </g>
                        <g>
                            <circle class="n-halo h3" cx="70" cy="360" r="14" fill="none" stroke="#34d399" stroke-width="0.8"/>
                            <circle class="n n3" cx="70" cy="360" r="7" fill="#34d399"/>
                            <text class="lbl l3" x="70" y="392" text-anchor="middle" font-size="10" fill="#8fa89c" font-family="system-ui">Proteins</text>
                        </g>
                        <g>
                            <circle class="n-halo h4" cx="330" cy="360" r="14" fill="none" stroke="#4ade80" stroke-width="0.8"/>
                            <circle class="n n4" cx="330" cy="360" r="7" fill="#4ade80"/>
                            <text class="lbl l4" x="330" y="392" text-anchor="middle" font-size="10" fill="#8fa89c" font-family="system-ui">Variants</text>
                        </g>
                        <g>
                            <circle class="n-halo h5" cx="200" cy="55" r="12" fill="none" stroke="#60a5fa" stroke-width="0.8"/>
                            <circle class="n n5" cx="200" cy="55" r="6" fill="#60a5fa"/>
                            <text class="lbl l5" x="200" y="34" text-anchor="middle" font-size="9" fill="#8fa89c" font-family="system-ui">Pathways</text>
                        </g>
                        <g>
                            <circle class="n-halo h6" cx="200" cy="395" r="12" fill="none" stroke="#34d399" stroke-width="0.8"/>
                            <circle class="n n6" cx="200" cy="395" r="6" fill="#34d399"/>
                            <text class="lbl l6" x="200" y="422" text-anchor="middle" font-size="9" fill="#8fa89c" font-family="system-ui">Compounds</text>
                        </g>
                        <g>
                            <circle class="n-halo h7" cx="55" cy="220" r="12" fill="none" stroke="#a7f3d0" stroke-width="0.8"/>
                            <circle class="n n7" cx="55" cy="220" r="6" fill="#a7f3d0"/>
                            <text class="lbl l7" x="40" y="200" text-anchor="middle" font-size="9" fill="#8fa89c" font-family="system-ui">Trials</text>
                        </g>
                        <g>
                            <circle class="n-halo h8" cx="345" cy="220" r="12" fill="none" stroke="#4ade80" stroke-width="0.8"/>
                            <circle class="n n8" cx="345" cy="220" r="6" fill="#4ade80"/>
                            <text class="lbl l8" x="360" y="200" text-anchor="middle" font-size="9" fill="#8fa89c" font-family="system-ui">Structures</text>
                        </g>
                    </svg>
                </div>

                <div class="web-side">
                    <div class="web-badge">
                        <svg width="14" height="14" viewBox="0 0 14 14"><circle cx="7" cy="7" r="5" fill="none" stroke="#4ade80" stroke-width="1.5"/><circle cx="7" cy="7" r="2" fill="#4ade80"/></svg>
                        Hundreds of curated sources
                    </div>
                    <h3>Reputable <span class="accent">URLs</span>, continuously read</h3>
                    <p>
                        Peer-reviewed publications, national reference databases,
                        protein structure archives, clinical trial registries.
                        Each source is vetted. Each new finding updates the graph.
                    </p>

                    <div class="web-categories">
                        <div class="web-cat">
                            <div class="label">Publications</div>
                            <div class="desc">Peer-reviewed findings</div>
                        </div>
                        <div class="web-cat">
                            <div class="label">Genomes</div>
                            <div class="desc">Reference assemblies</div>
                        </div>
                        <div class="web-cat">
                            <div class="label">Proteins</div>
                            <div class="desc">Structures and functions</div>
                        </div>
                        <div class="web-cat">
                            <div class="label">Variants</div>
                            <div class="desc">Population + clinical</div>
                        </div>
                        <div class="web-cat">
                            <div class="label">Compounds</div>
                            <div class="desc">Bioactivity + libraries</div>
                        </div>
                        <div class="web-cat">
                            <div class="label">Trials</div>
                            <div class="desc">Clinical registries</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="scan-visual">
            <h3>The continuous loop</h3>
            <div class="scan-flow">
                <div class="scan-step">
                    <span class="icon">🌐</span>
                    <div class="label">Crawl</div>
                    <div class="desc">Hundreds of curated URLs</div>
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
                    <div class="desc">Learn from new evidence</div>
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

<section id="validation">
    <div class="container">
        <h2>Validated <span class="accent">end to end</span></h2>
        <p class="lead">
            Patterns aren't just learned — they're stress-tested. Every
            model is verified across independent axes before it earns a
            place in the pipeline.
        </p>

        <div class="validation-grid">
            <div class="validation-card">
                <div class="icon-wrap">
                    <svg width="36" height="36" viewBox="0 0 40 40">
                        <circle cx="20" cy="20" r="14" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <path d="M8,20 Q20,12 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <path d="M8,20 Q20,28 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <circle cx="20" cy="20" r="3" fill="#a7f3d0"/>
                    </svg>
                </div>
                <h3>Cross-species</h3>
                <p>Models are validated against genomic structure from multiple species. A pattern that holds across evolutionary distance is more likely to reflect real biology.</p>
                <span class="meta">Cross-species</span>
            </div>

            <div class="validation-card">
                <div class="icon-wrap">
                    <svg width="36" height="36" viewBox="0 0 40 40">
                        <circle cx="14" cy="18" r="6" fill="none" stroke="#60a5fa" stroke-width="1.5"/>
                        <circle cx="26" cy="18" r="6" fill="none" stroke="#60a5fa" stroke-width="1.5"/>
                        <circle cx="20" cy="30" r="6" fill="none" stroke="#60a5fa" stroke-width="1.5"/>
                        <line x1="17" y1="22" x2="20" y2="25" stroke="#60a5fa" stroke-width="1.5"/>
                        <line x1="23" y1="22" x2="20" y2="25" stroke="#60a5fa" stroke-width="1.5"/>
                    </svg>
                </div>
                <h3>Animal models</h3>
                <p>Predictions are run against established animal disease models. Simulated outcomes are compared to real physiological responses from published studies.</p>
                <span class="meta">In vivo</span>
            </div>

            <div class="validation-card">
                <div class="icon-wrap">
                    <svg width="36" height="36" viewBox="0 0 40 40">
                        <rect x="8" y="10" width="24" height="20" rx="3" fill="none" stroke="#a7f3d0" stroke-width="1.5"/>
                        <line x1="20" y1="10" x2="20" y2="14" stroke="#a7f3d0" stroke-width="1.5"/>
                        <line x1="20" y1="26" x2="20" y2="30" stroke="#a7f3d0" stroke-width="1.5"/>
                        <line x1="16" y1="20" x2="24" y2="20" stroke="#a7f3d0" stroke-width="1.5"/>
                    </svg>
                </div>
                <h3>Human trial models</h3>
                <p>Protocols are evaluated against human clinical trial data — dosing, outcomes, adverse events, and time-to-response across published cohorts.</p>
                <span class="meta">Clinical</span>
            </div>

            <div class="validation-card">
                <div class="icon-wrap">
                    <svg width="36" height="36" viewBox="0 0 40 40">
                        <path d="M6,32 L6,24 L12,24 L12,18 L18,18 L18,26 L24,26 L24,14 L30,14 L30,10 L34,10" fill="none" stroke="#34d399" stroke-width="2" stroke-linejoin="round"/>
                        <circle cx="6" cy="32" r="2" fill="#34d399"/>
                        <circle cx="34" cy="10" r="2" fill="#34d399"/>
                    </svg>
                </div>
                <h3>Holdout evaluation</h3>
                <p>Models are tested on chromosomes, diseases, and compounds never seen during training. If performance holds, the pattern generalizes.</p>
                <span class="meta">Held-out</span>
            </div>
        </div>
    </div>
</section>

<section id="validation">
    <div class="container">
        <h2>Validated <span class="accent">end to end</span></h2>
        <p class="lead">
            Patterns aren't just learned — they're stress-tested. Every
            model is verified across independent axes before it earns a
            place in the pipeline.
        </p>

        <div class="validation-grid">
            <div class="validation-card">
                <div class="icon-wrap">
                    <svg width="36" height="36" viewBox="0 0 40 40">
                        <circle cx="20" cy="20" r="14" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <path d="M8,20 Q20,12 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <path d="M8,20 Q20,28 32,20 T8,20" fill="none" stroke="#4ade80" stroke-width="1.5"/>
                        <circle cx="20" cy="20" r="3" fill="#a7f3d0"/>
                    </svg>
                </div>
                <h3>Cross-species</h3>
                <p>Models are validated against genomic structure from multiple species. A pattern that holds across evolutionary distance is more likely to reflect real biology.</p>
                <span class="meta">Cross-species</span>
            </div>

            <div class="validation-card">
                <div class="icon-wrap">
                    <svg width="36" height="36" viewBox="0 0 40 40">
                        <circle cx="14" cy="18" r="6" fill="none" stroke="#60a5fa" stroke-width="1.5"/>
                        <circle cx="26" cy="18" r="6" fill="none" stroke="#60a5fa" stroke-width="1.5"/>
                        <circle cx="20" cy="30" r="6" fill="none" stroke="#60a5fa" stroke-width="1.5"/>
                        <line x1="17" y1="22" x2="20" y2="25" stroke="#60a5fa" stroke-width="1.5"/>
                        <line x1="23" y1="22" x2="20" y2="25" stroke="#60a5fa" stroke-width="1.5"/>
                    </svg>
                </div>
                <h3>Animal models</h3>
                <p>Predictions are run against established animal disease models. Simulated outcomes are compared to real physiological responses from published studies.</p>
                <span class="meta">In vivo</span>
            </div>

            <div class="validation-card">
                <div class="icon-wrap">
                    <svg width="36" height="36" viewBox="0 0 40 40">
                        <rect x="8" y="10" width="24" height="20" rx="3" fill="none" stroke="#a7f3d0" stroke-width="1.5"/>
                        <line x1="20" y1="10" x2="20" y2="14" stroke="#a7f3d0" stroke-width="1.5"/>
                        <line x1="20" y1="26" x2="20" y2="30" stroke="#a7f3d0" stroke-width="1.5"/>
                        <line x1="16" y1="20" x2="24" y2="20" stroke="#a7f3d0" stroke-width="1.5"/>
                    </svg>
                </div>
                <h3>Human trial models</h3>
                <p>Protocols are evaluated against human clinical trial data — dosing, outcomes, adverse events, and time-to-response across published cohorts.</p>
                <span class="meta">Clinical</span>
            </div>

            <div class="validation-card">
                <div class="icon-wrap">
                    <svg width="36" height="36" viewBox="0 0 40 40">
                        <path d="M6,32 L6,24 L12,24 L12,18 L18,18 L18,26 L24,26 L24,14 L30,14 L30,10 L34,10" fill="none" stroke="#34d399" stroke-width="2" stroke-linejoin="round"/>
                        <circle cx="6" cy="32" r="2" fill="#34d399"/>
                        <circle cx="34" cy="10" r="2" fill="#34d399"/>
                    </svg>
                </div>
                <h3>Holdout evaluation</h3>
                <p>Models are tested on chromosomes, diseases, and compounds never seen during training. If performance holds, the pattern generalizes.</p>
                <span class="meta">Held-out</span>
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
        <h2>How compounds are <span class="accent">scored</span></h2>
        <p class="lead">
            Every compound-target pair is evaluated from multiple angles.
            Each contributes evidence. Together they produce one ranking.
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
