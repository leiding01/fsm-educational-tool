# Variant 3 – Replication & Consistency Models Tool (One‑page Brief)

Student: Lei Ding (K21029011) · Supervisor: Dr Angelos Georgoulas
Module: 6CCS3PRJ · First meeting: Thu 6 Nov 2025, 15:00–16:00, Bush House (N) 7.11

Goal & Scope (small, reproducible)
- A lightweight web simulator to contrast strong / causal / eventual consistency on 3–5 replicas.
- Read/write operations; step/auto‑play; per‑step message log; JSON/PNG export.
- Optional toggles: delay/partition; highlight anomalies (stale read, read‑your‑writes).
- Out of scope: full database implementation; complex animations; large user studies.

Architecture
- replica_core.js: model, consistency rules, anomaly detectors.
- replica_main.js: UI (swimlanes & arrows), step/play controls, log, import/export.
- Stack: HTML/JS/CSS (no runtime deps); deploy via GitHub Pages.

Evaluation
- Correctness: black‑box scenarios (sequential / concurrent / partition+repair) with expected outcomes.
- Performance: small rendering/playback timing table (3× repeats).
- Usability: Nielsen heuristic checklist with 6–8 screenshots.
- Reproducibility: all scenarios as JSON; figures as PNG; README with one‑click run.

Plan (4 weeks)
- W1: model & scenarios; strong & eventual; message log.
- W2: UI swimlanes; step/auto‑play; import/export.
- W3: causal rule; anomaly detectors; figures.
- W4: evaluation (tests/timing/Nielsen); documentation.
