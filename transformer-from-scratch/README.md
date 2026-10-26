# Transformer from Scratch → LoRA Fine-tune

A small decoder-only transformer built from first principles, followed by parameter-efficient fine-tuning (LoRA / QLoRA) of a small pretrained open model.

**Why this project:** to understand transformer internals by implementing them, not just calling them — and to connect that to the modern fine-tuning ecosystem. Built alongside interview prep; the write-up at the end doubles as a talking script.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_GITHUB_USERNAME/transformer-from-scratch/blob/main/notebooks/01_attention_from_scratch.ipynb)
<!-- Replace YOUR_GITHUB_USERNAME above after you create the repo -->

---

## Roadmap

| Week | Milestone | Status |
|---|---|---|
| 1–2 | Scaled dot-product + multi-head attention from scratch (NumPy → PyTorch), with tests | ⬜ |
| 3 | Full transformer block (pre-norm, MLP, residuals); overfit a tiny dataset to prove correctness | ⬜ |
| 4 | Train a small model on a char/token dataset; sample from it; log curves to wandb | ⬜ |
| 5 | Fine-tune a small pretrained model with LoRA / QLoRA on a focused task | ⬜ |
| 6 | Evaluate (held-out metric + qualitative samples); write up results below | ⬜ |

## Repo layout

```
notebooks/   exploratory work, one notebook per milestone
src/         reusable modules (attention, block, model, train loop) — from Week 3–4
LOG.md       short session journal: what I did, what confused me, interview-worthy insights
SETUP.md     environment setup checklist
```

## Running

Training runs in Google Colab (free T4 GPU for Weeks 1–4; Colab Pro for the Week 5–6 fine-tune). Click the badge above, or in Colab: **File → Open notebook → GitHub**.

---

## Results

*(Filled in Week 6: problem, approach, results table/plot, limitations, what I'd do next.)*
