# Setup Checklist

Do this once, in your first session (~30 min). Then spend the rest of the session on the notebook.

## 1. GitHub repo (10 min)

1. On github.com → **New repository** → name it `transformer-from-scratch`, **Public**, no template, don't add a README (you already have one).
2. Add these files — pick one route:
   - **No local tools:** on the empty repo page click **"uploading an existing file"**, drag in everything from this folder (keep the `notebooks/` and `src/` folders), commit.
   - **With Git installed locally:**
     ```bash
     cd transformer-from-scratch
     git init && git add . && git commit -m "Initial scaffold"
     git branch -M main
     git remote add origin https://github.com/<your-username>/transformer-from-scratch.git
     git push -u origin main
     ```
3. In `README.md`, replace `YOUR_GITHUB_USERNAME` in the Colab badge link with your username.

## 2. Colab (10 min)

1. Open colab.research.google.com → **File → Open notebook → GitHub** tab → authorize GitHub → pick your repo → `notebooks/01_attention_from_scratch.ipynb`.
2. **Runtime:** CPU is fine for this first notebook. From Week 3 onward, use **Runtime → Change runtime type → T4 GPU**.
3. **Turn off AI code completion** in Colab's settings (Tools → Settings) for the from-scratch sessions. Frontier-lab coding rounds prohibit AI assistance, so build the unaided muscle now. (Turn it back on for Week 5's LoRA plumbing if you want.)
4. **Saving — important:** Colab does *not* auto-sync to GitHub. At the end of every session: **File → Save a copy in GitHub** → same repo, same path → write a meaningful commit message (e.g. "MHA passes reference test"). Your commit history becomes part of the portfolio story.

## 3. Weights & Biases (5 min — can wait until Week 4)

1. Sign up at wandb.ai (free for personal use).
2. Copy your API key from your user settings.
3. In Colab, store it under the 🔑 **Secrets** panel (left sidebar) as `WANDB_API_KEY` — never paste keys into notebook cells that get pushed to GitHub.

## 4. Local tools (optional)

- **VS Code** with the Python + Jupyter extensions, and **Git** — useful from Week 3–4, when code moves from notebooks into `src/*.py`. Not needed for Session 1.

## Session habit

Last 5 minutes of every session: add 3 lines to `LOG.md` (did / confused by / interview insight), then save to GitHub. It makes restarting the next session fast, and Week 6's write-up almost writes itself.
