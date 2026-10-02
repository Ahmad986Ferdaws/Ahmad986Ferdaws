<div align="center">

# Ahmad Ferdaws Shafiq

<a href="https://ferdaws.dev"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=3200&pause=1000&color=58A6FF&center=true&vCenter=true&width=640&lines=I+build+ML+systems+that+know+when+to+say+%22I+don%27t+know.%22;Sealed+test+sets.+Calibrated+confidence.+Honest+results.;From+research+notebook+to+tested%2C+shipped+software." alt="I build ML systems that know when to say I don't know" /></a>

[![Portfolio](https://img.shields.io/badge/ferdaws.dev-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://ferdaws.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/ferdaws3440)

</div>

I build machine learning for settings where a confident wrong answer is expensive: models that abstain when unsure, evaluations that can't leak, and results I report even when the answer is *no*.

### ⚡ Featured work

| Project | What it proves |
|:--|:--|
| **[ECG Trust Lab](https://github.com/Ahmad986Ferdaws/ecg-trust-lab)**<br><sub>PyTorch · FastAPI · Plotly</sub> | 12-lead ECG classifier on PTB-XL (21K ECGs, 18K patients) scored once on a sealed test fold: **0.922 macro-AUROC**, calibrated probabilities, and a confidence gate that defers uncertain cases to a human. The frozen models then hit **0.931 AUROC on a second, independent dataset with zero retuning**. 494 automated tests, strict mypy. |
| **[REGIME](https://github.com/Ahmad986Ferdaws/markov_selflearning_trade)**<br><sub>Python · GitHub Actions</sub> | My trading model scored **90.9%**, so I built a harness to try to break it. Across **20 markets, 20 years of history and 16,773 held-out predictions**, its edge over the naive *"tomorrow = today"* baseline is **exactly zero**. Positive controls in CI prove the harness catches a real edge when one exists. |
| **[FoodVisor AI](https://github.com/Ahmad986Ferdaws/food_visor_ai)**<br><sub>FastAPI · Next.js · pgvector · Celery</sub> | Three cooperating LLM agents (context → recommend → validate) over **pgvector RAG**, with long-running jobs on Celery + Redis. The full stack comes up with one `docker compose up`. |
| **[Cortex BCI Visualizer](https://github.com/Ahmad986Ferdaws/Neuron-cortex-simulation-model)**<br><sub>React Three Fiber · TypeScript</sub> | **Rice Datathon 2026.** A 3D head model that polls our team's EEGNet motor-imagery model every 250 ms and lights up the matching motor-cortex electrodes. The model reads 4 movement intentions from raw 64-channel EEG at **42% vs 25% chance, on unseen subjects**. |

### 🧭 How I work

- **Sealed evaluation.** The final test set is touched once. Calibration and thresholds get their own data.
- **Receipts over vibes.** A null result with evidence beats an impressive number nobody checked.
- **Ship it end to end.** Typed code, tests, CI, Docker, and a demo you can actually click.

### 🛠️ Stack

<img src="https://skillicons.dev/icons?i=py,pytorch,tensorflow,sklearn,fastapi,postgres,redis,docker,aws,azure&theme=dark" alt="Python, PyTorch, TensorFlow, scikit-learn, FastAPI, PostgreSQL, Redis, Docker, AWS, Azure" /><br>
<img src="https://skillicons.dev/icons?i=ts,react,nextjs,tailwind,threejs,nodejs,githubactions,git,linux&theme=dark" alt="TypeScript, React, Next.js, Tailwind, Three.js, Node.js, GitHub Actions, Git, Linux" />

<sub>Also: LLM agents · RAG · LangChain · pgvector · Celery · Prisma · MNE-Python · calibration & conformal methods</sub>
