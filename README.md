# Satyabrat Mishra

*B.Tech CSE (Artificial Intelligence & Machine Learning)*

I build practical engineering systems that combine software, AI/ML, and real-world data.

---

### What I build

- AI/ML systems trained and validated against real, messy, publicly-sourced data, not toy datasets
- Full-stack applications with a real frontend, backend, and database, taken through to a working deployment
- Geospatial and environmental data pipelines: terrain, satellite rainfall, and field-survey data joined into one system
- Engineering work that states its own limitations: what's measured, what's assumed, and what's still a prototype

---

### Featured projects

**STRIDE-X** - *Spatiotemporal Terrain Risk Intelligence & Dynamic Early-warning System*  
AI-based landslide risk-monitoring system for India's North Eastern Region.

`Terrain + Rainfall + Ground Evidence → Explainable Risk → Road-level Action`

- **36,071** GSI landslide records + SRTM terrain + NASA IMERG rainfall + geospatial road data
- Spatially blocked validation and **road-survey bias auditing** before modelling
- Designed citizen-photo evidence with bounded, time-decaying influence and explicit provenance
- **55 end-to-end assertions, 0 failing**

*Private during evaluation.*

**[SAWA](https://github.com/Enigmasatyabrat/SAWA)** - *Soil Analysis Web App*
Full-stack computer-vision pipeline that classifies soil type and estimates pH/N-P-K levels from a photo, then recommends crops.

- K-means colour clustering drives soil classification and nutrient estimation
- A client-side validation gate rejects non-soil images and flags low-confidence results as uncertain instead of guessing, and attaches a confidence score and its evidence to every result
- Next.js App Router, TypeScript, MongoDB: real server-side API routes, not a static export
- Rebuilt from an earlier React + FastAPI version, with the migration reasoning documented rather than left implicit

**[StockFlow](https://github.com/Enigmasatyabrat/StockFlow)** - *Marketplace Photo Pipeline*
CLI tool that scores, sorts, and prepares photography for stock marketplaces end to end.

- Measures real technical quality (sharpness, noise, exposure, contrast) with NumPy before a vision model judges commercial prospects: measurement first, model opinion second
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

Building AI/ML systems that connect software with real-world data, with a growing focus on geospatial and environmental intelligence.

---

### Contact

- GitHub: [@Enigmasatyabrat](https://github.com/Enigmasatyabrat)
