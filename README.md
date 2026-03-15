 Sparse Semantic Patch Memory (SSPM)

This repository contains the **proof-of-concept implementation and experimental notebook** for the research work:

**Token-Efficient Conversational History Management using Sparse Semantic Patch Memory (SSPM).**

SSPM proposes a **semantic patch–based memory architecture** for Large Language Models that reduces token usage while preserving critical conversational constraints and decisions.

---

 Research Paper

The full research preprint is available in this repository:

```
paper/SSPM_v1_preprint.pdf
```

---

 Run the Experiment (Google Colab)

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

 Repository Structure

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

 Key Results

Average results from experiments:

| Method              | Avg Tokens Stored | Token Reduction |
| ------------------- | ----------------- | --------------- |
| Raw History         | 487               | 0%              |
| Token Truncation    | 298               | 38.8%           |
| Token Compression   | 312               | 35.9%           |
| **SSPM (Proposed)** | **249**           | **48.7%**       |

SSPM preserved **100% of constraints and decisions** across all evaluated dialogues.

---

 Citation

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
