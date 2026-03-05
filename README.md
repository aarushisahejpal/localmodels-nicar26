# Local Models — NICAR 2026

Notebooks for running LLMs locally via [LM Studio](https://lmstudio.ai). Requires a model loaded in LM Studio at `http://localhost:1234`.

## Installation

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Then open [LM Studio](https://lmstudio.ai), load a model, and start the local server on `http://localhost:1234`.

## Notebooks

- `1-semantic-map.ipynb` — Embeds NICAR session descriptions and plots them as a 2D semantic map.
- `2-classification.ipynb` — Classifies sessions using a local LLM with a yes/no prompt.
- `3-clustering.ipynb` — Clusters session embeddings with HDBSCAN and names each cluster using a local LLM.
- `4-conflicts-of-interest.ipynb` — Extracts author–company conflict relationships from a COI statement into a table.
- `5-conflict-of-interest-structured-outputs.ipynb` — Same as #4 but uses a JSON schema to guarantee structured, parseable output.