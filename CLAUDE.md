# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a research project using **graphify** to generate knowledge graphs from academic papers about seismic inversion, geophysics, and deep learning. The project contains two main analysis outputs:

1. **Papers Analysis** (`graphify-out/`) - Knowledge graph of seismic inversion research papers (322 nodes, 393 edges, 24 communities)
2. **CBA Congress Temporal KG** (`CBA congresso temporal kg/`) - Temporal knowledge graph of conference proceedings from 1998-2004 (314 nodes, 659 edges)

## Environment Setup

**Python Virtual Environment:**
```bash
source venv/bin/activate
```

All Python commands must be run with the virtual environment activated. Chain commands using `&&` to maintain the activated environment:
```bash
source venv/bin/activate && python script.py
```

**Installed Package:**
- `graphifyy==0.5.5` - Knowledge graph generation tool

## Project Structure

```
.
├── graphify-out/              # Main knowledge graph output
│   ├── GRAPH_REPORT.md       # Human-readable graph analysis
│   ├── graph.json            # NetworkX JSON graph with hyperedges
│   ├── manifest.json         # File timestamps and metadata
│   └── cost.json             # Token usage statistics
│
├── CBA congresso temporal kg/ # Temporal knowledge graph analysis
│   ├── graphify-out/         # Graphify output for CBA papers
│   └── temporal-kg/
│       ├── temporal_knowledge_graph.json  # Temporal graph (Articles, Authors, Affiliations, etc.)
│       └── AUDIT.md          # Extraction notes and statistics
│
└── venv/                      # Python virtual environment
```

## Knowledge Graph Architecture

### Papers Knowledge Graph (graphify-out/)

**Domain:** Seismic inversion and deep learning research

**Key Communities:**
1. Bayesian Seismic Inversion (52 nodes)
2. FWI & Deep Learning (46 nodes) - Full Waveform Inversion methods
3. Velocity Model Building (37 nodes)
4. Seismic Fault Interpretation (37 nodes)
5. GAN Seismic Noise Attenuation (17 nodes)

**Graph Features:**
- Contains hyperedges representing complex relationships between multiple papers
- Tracks EXTRACTED, INFERRED, and AMBIGUOUS edge types
- Identifies "God Nodes" (highly connected hub papers) and bridge papers
- Community detection using clustering algorithms

**Top Hub Papers:**
- Hosseinzadeh et al. 2025 (43 edges) - Seismic inversion review
- Dong et al. 2024 (24 edges) - Ediacaran paleoenvironment
- Lin et al. 2023 (23 edges) - Physics-guided data-driven FWI

### Temporal Knowledge Graph (CBA congresso temporal kg/)

**Domain:** Conference proceedings analysis (CBA 1998-2004)

**Node Types:** Article, Author, Affiliation, Keyword, Theme, Year

**Edge Types:** Was_Author_of, Is_Linked_to, Contains, Was_Associated_To, Has_Expertise_In, Next_Time, Collaborates, Was_Published_In

**Key Features:**
- Temporal evolution tracking across conference years
- Author collaboration networks
- Expertise and keyword extraction
- Mixed directed/undirected edges (Collaborates edges are undirected)

## Working with Graphify Output

### Graph Report Structure

The `GRAPH_REPORT.md` files contain:
- **Corpus Check:** Size and context window fit
- **Summary:** Node/edge counts, extraction quality, token costs
- **Community Hubs:** Major research clusters
- **God Nodes:** Most connected entities
- **Surprising Connections:** Unexpected relationships between papers
- **Hyperedges:** Group relationships (multi-node patterns)
- **Ambiguous Edges:** Low-confidence connections requiring review
- **Knowledge Gaps:** Isolated nodes and thin communities

### Graph JSON Format

`graph.json` uses NetworkX JSON format with custom extensions:
- **Hyperedges:** Complex multi-node relationships with confidence scores
- **Edge metadata:** `confidence` (EXTRACTED/INFERRED/AMBIGUOUS), `confidence_score`, `source_file`
- **Node metadata:** Paper titles, concepts, authors, institutions

## Git Configuration

**.gitignore:** Currently only ignores `papers/` directory

The following directories contain generated outputs and are committed:
- `graphify-out/` (612K)
- `CBA congresso temporal kg/` (924K)

## Common Workflows

### Analyzing Graph Structure
Read `GRAPH_REPORT.md` for high-level insights about communities, hubs, and knowledge gaps.

### Exploring Relationships
Use `graph.json` to programmatically traverse edges, filter by confidence scores, or analyze hyperedges.

### Understanding Extraction Quality
Check the Summary section in `GRAPH_REPORT.md`:
- High percentage of EXTRACTED edges = direct evidence from papers
- INFERRED edges have confidence scores (0.0-1.0)
- AMBIGUOUS edges need manual review

### Temporal Analysis
The temporal knowledge graph in `CBA congresso temporal kg/temporal-kg/temporal_knowledge_graph.json` tracks evolution over time using Year nodes and Next_Time edges.

## Data Quality Notes

### Papers Graph
- 96% EXTRACTED, 3% INFERRED, 1% AMBIGUOUS
- 11 inferred edges with average confidence 0.82
- 3 ambiguous edges requiring review (B1, B2, B4 papers - file access issues)
- 42 isolated nodes with ≤1 connection

### Temporal Graph
- 20 articles processed from years 1998, 2000, 2002, 2004
- Common extraction issues: missing abstracts, missing keywords, missing affiliations
- Article-level affiliation mapping used when PDF layout is ambiguous

## Research Domains

**Primary Focus:**
- Full Waveform Inversion (FWI)
- Physics-guided machine learning for seismics
- Bayesian uncertainty quantification
- Deep learning architectures (GANs, CNNs, PINNs)
- Velocity model building
- Seismic fault interpretation

**Key Technologies:**
- Physics-Informed Neural Networks (PINNs)
- Generative Adversarial Networks (GANs)
- Convolutional Neural Networks (CNNs)
- Bayesian inference frameworks
- OpenFWI benchmark datasets
