# Sparse Semantic Patch Memory (SSPM)

This repository contains the **proof-of-concept implementation and experimental notebook** for the research work:

**Token-Efficient Conversational History Management using Sparse Semantic Patch Memory (SSPM).**

SSPM proposes a **semantic patch–based memory architecture** for Large Language Models that reduces token usage while preserving critical conversational constraints and decisions.

---

## Research Paper

The full research preprint is available in this repository:

```
paper/SSPM_v1_preprint.pdf
```

---

## Run the Experiment (Google Colab)

You can run the full experiment directly in Google Colab:

**Launch Notebook:**
https://colab.research.google.com/drive/1fghj8UGg6bUTD5lunB9YxFo9B3f8GIwi

The notebook performs:

* Dialogue generation
* Semantic patch extraction
* Utility scoring
* Sparse patch selection
* Experimental evaluation
* Result visualization

---

## Repository Structure

```
Sparse-Semantic-Patch-Memory-SSPM-Proof-of-Concept
│
├── diagrams/
│   └── architecture.png
│
├── notebooks/
│   └── SSPM_experiment.ipynb
│
├── paper/
│   └── SSPM_v1_preprint.pdf
│
└── README.md
```

---

## Key Results

Average results from experiments:

| Method              | Avg Tokens Stored | Token Reduction |
| ------------------- | ----------------- | --------------- |
| Raw History         | 487               | 0%              |
| Token Truncation    | 298               | 38.8%           |
| Token Compression   | 312               | 35.9%           |
| **SSPM (Proposed)** | **249**           | **48.7%**       |

SSPM preserved **100% of constraints and decisions** across all evaluated dialogues.

---

## Experimental Results

The proof-of-concept implementation of **Sparse Semantic Patch Memory (SSPM)** was evaluated on multiple multi-turn technical dialogues under a fixed token budget.

The experiments demonstrate that SSPM significantly reduces conversational token usage while preserving important semantic information such as constraints and decisions.

The figure below summarizes the experimental results including token usage comparison, semantic patch extraction statistics, token reduction percentage, and ablation analysis.

![SSPM Experimental Results](results/SSPM_Results.png)

**Key findings:**

* SSPM achieves **~48.7% average token reduction** compared to raw conversation history.
* All explicit **constraints and decisions are preserved (100% retention)**.
* Sparse semantic patch selection improves efficiency compared to truncation and compression baselines.
* Ablation experiments confirm the importance of **dependency centrality and token cost penalty** in the utility scoring function.

## Citation

If you use this work, please cite:

```
Dubey, D. (2026).
Token-Efficient Conversational History Management using Sparse Semantic Patch Memory.
Zenodo.
https://doi.org/10.5281/zenodo.18849304
```

---

## License

MIT License
