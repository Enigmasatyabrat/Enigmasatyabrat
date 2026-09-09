# Satyabrat Mishra

*B.Tech CSE (Artificial Intelligence & Machine Learning)*
I build practical engineering systems that combine software, AI/ML, and real-world data.

---

### What I build

- AI/ML systems trained and validated against real, messy, publicly-sourced data - not toy datasets
- Full-stack applications with a real frontend, backend, and database, taken through to a working deployment
- Geospatial and environmental data pipelines: terrain, satellite rainfall, and field-survey data joined into one system
- Engineering work that states its own limitations - what's measured, what's assumed, and what's still a prototype

---

### Featured projects

**STRIDE-X** - *Spatiotemporal Terrain Risk Intelligence & Dynamic Early-warning System*
AI-based landslide early-warning prototype for India's North Eastern Region, built for Smart India Hackathon 2026 (Problem Statement 26001, Ministry of DoNER).

`Terrain + Rainfall + Ground Evidence → Explainable Risk → Road-level Action`

- Susceptibility model fitted on SRTM-derived terrain features against **36,071** GSI field-validated landslide records, using spatially blocked cross-validation to avoid geographic leakage
- Audited the source inventory for road-survey bias before modelling: Mizoram's 3,486 recorded landslides sit a **median 16 m** from a road, against **873 m** for 20,000 random points in the same state - removed the confounded distance-to-road feature and road-distance-matched the negative samples instead of ignoring the finding
- Rainfall trigger layer built on real NASA GPM IMERG data; **1,500** of 11,026 NER records carry a day-level date usable for rainfall-event alignment
- Designed - not yet trained - a citizen-photo evidence layer: bounded, time-decaying influence on the risk score, with provenance reported for every input (real, assumed, or mock).
- **55 end-to-end assertions, 0 failing** (verified locally): the full evidence-submission loop, before/after arithmetic, tamper rejection, and edge cases, run against a live server

*Private during evaluation.*

**[SAWA](https://github.com/Enigmasatyabrat/SAWA)** - *Soil Analysis Web App*
Full-stack computer-vision pipeline that classifies soil type and estimates pH/N-P-K levels from a photo, then recommends crops.

- K-means colour clustering drives soil classification and nutrient estimation
- A client-side validation gate rejects non-soil images and flags low-confidence results as uncertain instead of guessing - attaches a confidence score and its evidence to every result
- Next.js App Router, TypeScript, MongoDB - real server-side API routes, not a static export
- Rebuilt from an earlier React + FastAPI version, with the migration reasoning documented rather than left implicit

**[StockFlow](https://github.com/Enigmasatyabrat/StockFlow)** - *Marketplace Photo Pipeline*
CLI tool that scores, sorts, and prepares photography for stock marketplaces end to end.

- Measures real technical quality (sharpness, noise, exposure, contrast) with NumPy before a vision model judges commercial prospects - measurement first, model opinion second
- Resumable and crash-safe: journals every file move, tracks pending work across interrupted runs
- Threshold calibration against your own accepted/rejected photo history, not hardcoded defaults
- 8 tagged releases, changelog, roadmap, and a test suite that runs with no API key and no network

---

### Technical focus

| | |
|---|---|
| **Languages** | Python, JavaScript, TypeScript |
| **ML / data** | scikit-learn, spatially-aware cross-validation, K-means clustering, NumPy-based signal measurement, vision-model integration |
| **Full-stack** | Next.js, React, FastAPI, Node.js, MongoDB |
| **Geospatial & environmental data** | SRTM elevation, NASA GPM IMERG rainfall, OpenStreetMap, GSI survey data |
| **Engineering practice** | automated end-to-end testing, versioned releases, bias auditing, documented architecture and limitations |

---

### Current direction

Geospatial and environmental AI systems - models that hold up against real, biased, incomplete field data rather than clean benchmarks.

---

### Contact

- GitHub: [@Enigmasatyabrat](https://github.com/Enigmasatyabrat)
