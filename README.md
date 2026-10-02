<div align="center">

# Ahmad Ferdaws Shafiq

<a href="https://ferdaws.dev"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=3200&pause=1000&color=58A6FF&center=true&vCenter=true&width=640&lines=I+build+ML+systems+that+know+when+to+say+%22I+don%27t+know.%22;Sealed+test+sets.+Calibrated+confidence.+Honest+results.;From+research+notebook+to+tested%2C+shipped+software." alt="I build ML systems that know when to say I don't know" /></a>

[![Portfolio](https://img.shields.io/badge/ferdaws.dev-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://ferdaws.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/ferdaws3440)

</div>

I build machine learning for settings where a confident wrong answer is expensive: models that abstain when unsure, evaluations that can't leak, and results I report even when the answer is *no*.

## 🔬 Projects

### 🫀 [ECG Trust Lab](https://github.com/Ahmad986Ferdaws/ecg-trust-lab): heart-signal AI you can audit
<sub>PyTorch · FastAPI · Plotly · pytest · mypy</sub>

Most ML projects stop at "the model is accurate." This one asks what it would take to *trust* it.

- Trained a 1D ResNet and an ECG transformer under the same budget on **21,388 ECGs from 18,617 patients** (PTB-XL), with no patient shared across splits.
- Scored once on a sealed test fold: **0.922 macro-AUROC**, with calibrated probabilities and a confidence gate that defers uncertain ECGs instead of guessing.
- Ran the frozen models **unchanged on a second dataset of 15.7K ECGs: 0.931 AUROC with zero retuning**.
- The audit surfaced what one score hides: the gate accepts only 60–65% of patients aged 80+ vs ~94% under 40, and reversed leads cause the worst failures.
- Local demo with the 12-lead waveform, calibrated scores, accept/defer decision and Grad-CAM overlay. **494 automated tests**, strict mypy.
- Now building **Trust Sentinel**: input-quality checks, unfamiliar-input detection, conformal uncertainty and fail-closed decisions.

### 📉 [REGIME](https://github.com/Ahmad986Ferdaws/markov_selflearning_trade): proving my own model has no edge
<sub>Python · GitHub Actions · walk-forward evaluation</sub>

My Markov regime trading model hit a **90.9%** hit rate. I built a harness to find out if that was real.

- It wasn't. Guessing *"tomorrow = today"* also scores **90.9%**, so the edge is **exactly zero**.
- The result held across **20 markets** and **20 years** of history, including 2008, COVID and the 2022 bear market: **0 differences in 16,773 held-out predictions**.
- Found the cause: the transition matrix is so sticky the model never predicts a change (**0 of 30** regime switches caught).
- Positive controls in CI prove the harness *does* catch a real edge when one is planted. Byte-reproducible from a fresh clone.

### 🥗 [FoodVisor AI](https://github.com/Ahmad986Ferdaws/food_visor_ai): multi-agent nutrition recommender
<sub>FastAPI · Next.js · PostgreSQL + pgvector · Celery · Redis · Docker</sub>

- Three LLM agents in a pipeline: one builds the user's context, one recommends meals, one checks the result against the user's constraints.
- Retrieval-augmented generation over a knowledge base stored as **pgvector** embeddings.
- Long agent runs go to **Celery** workers so the API stays fast. JWT auth, Alembic migrations, and the whole stack starts with one `docker compose up`.

### 🧠 [Cortex BCI Visualizer](https://github.com/Ahmad986Ferdaws/Neuron-cortex-simulation-model): Rice Datathon 2026
<sub>React Three Fiber · Three.js · TypeScript · EEGNet</sub>

- A 3D head model that sends 64-channel EEG trials to our team's model every 250 ms and lights up the matching motor-cortex electrodes.
- The EEGNet model reads 4 movement intentions (left hand, right hand, both hands, feet) from raw brain signals: **42% vs 25% chance, on people it never saw in training**.

### 🎓 [Admission Copilot](https://github.com/Ahmad986Ferdaws/Admission-Copilot): university program matching
<sub>Next.js 14 · TypeScript · Prisma · PostgreSQL · Gemini</sub>

- Matches students to programs on GPA, test scores, budget, location and major, then sorts them into **Safe / Match / Reach**.
- Gemini explains why each program fits, generates document checklists and builds a deadline-tracked task list.

## 🛠️ Stack

<img src="https://skillicons.dev/icons?i=py,pytorch,tensorflow,sklearn,fastapi,postgres,redis,docker,aws,azure&theme=dark" alt="Python, PyTorch, TensorFlow, scikit-learn, FastAPI, PostgreSQL, Redis, Docker, AWS, Azure" /><br>
<img src="https://skillicons.dev/icons?i=ts,react,nextjs,tailwind,threejs,nodejs,githubactions,git,linux&theme=dark" alt="TypeScript, React, Next.js, Tailwind, Three.js, Node.js, GitHub Actions, Git, Linux" />
