# Kepler-90 Outer Planets: Orbital Stability and Machine Learning Classification

This project investigates the long-term orbital stability of the outer planets in the Kepler-90 system (g, h, i) using N-body simulations. It also leverages machine learning to classify stable vs. unstable planetary configurations, merging computational astrophysics with data-driven techniques.

## Project Timeline and Structure

### Phase 1: Preliminary Research and Setup (Week 1)

**Background Research**
- Study the Kepler-90 planetary system, focusing on outer planets (g, h, i).
- Review fundamentals of N-body simulations and orbital mechanics.

**Data Collection**
- Retrieve planetary and stellar parameters from NASA Exoplanet Archive.

**Software Setup**
- Install required tools: `Rebound`, `AstroPy`, `NumPy`, `Matplotlib`.
- Install machine learning libraries: `scikit-learn`, `XGBoost`, `TensorFlow` (optional).

---

### Phase 2: Simulation Design and Setup (Week 2)

**Design Simulations**
- Define the simulation timeframe (e.g., 1 million years).
- Select Kepler-90 g, h, and i as focus planets.
- Specify initial conditions: mass, semi-major axis, eccentricity, inclination.

**Setup in Rebound**
- Input planetary parameters into the simulation environment.
- Choose an appropriate integrator (e.g., IAS15).
- Run small test simulations to validate the setup.

---

### Phase 3: Run Simulations (Weeks 3–4)

**Simulate Orbital Evolution**
- Run long-term N-body simulations.
- Track positions, velocities, and gravitational interactions.

**Data Collection**
- Log orbital parameters: eccentricity, semi-major axis, period, and inclination.
- Record data at fixed intervals (e.g., every 1,000 or 10,000 years).

**Sensitivity Analysis**
- Slightly vary initial conditions.
- Observe the effects on orbital stability.

---

### Phase 4: Machine Learning and Feature Engineering (Week 5)

**Feature Engineering**
- Structure the simulation output into a dataset.
- Input features: initial conditions and statistical descriptors (mean eccentricity, variance, close encounter counts).
- Output labels: “Stable” or “Unstable,” defined based on orbital criteria.

**Model Training**
- Train classification models:
  - `RandomForestClassifier` for binary stability classification.
  - `XGBoost` for higher accuracy.
  - Optional: `LSTM` models for time-series prediction.
- Evaluate models using accuracy, F1-score, and confusion matrix.

---

### Phase 5: Analysis and Interpretation (Week 6)

**Stability and Resonance Checks**
- Plot orbital variations over time.
- Detect orbital resonances using period ratios (e.g., 2:1, 3:2).

**Machine Learning Insights**
- Analyze feature importance to understand predictors of stability.
- Generate decision boundaries or 2D stability maps.

**Chaos Detection (Optional)**
- Identify chaotic behavior using ML models trained on sensitivity runs.

---

### Phase 6: Report Writing and Visualization (Weeks 7–8)

**Documentation**
- Introduction: Overview of Kepler-90 and motivation for using ML.
- Methodology: Detailed simulation and ML pipeline.
- Results: Model performance, orbital patterns, stability classifications.
- Discussion: Astrophysical implications and limitations.
- Conclusion: Key findings and suggestions for future work.

**Figures**
- Orbit evolution plots
- Eccentricity time-series
- Feature importance charts
- Confusion matrix from ML models

---

### Phase 7: Final Submission (End of Week 8)

**Formatting and Publishing**
- Prepare the manuscript using Overleaf or Google Docs.
- Target submission to journals such as:
  - The Astrophysical Journal (ApJ)
  - Monthly Notices of the Royal Astronomical Society (MNRAS)
  - Astronomy & Astrophysics (A&A)

---

## Optional Advanced Ideas

- Use AutoML tools like `TPOT` for model selection and tuning.
- Apply LSTM networks to predict future orbital states from sequences.
- Use dimensionality reduction techniques like PCA or t-SNE for visualization.

---

## Prerequisites

- Python 3.x
- Basic understanding of orbital mechanics and planetary dynamics
- Familiarity with Python libraries: `rebound`, `numpy`, `matplotlib`, `scikit-learn`, `xgboost`

---

## References

- NASA Exoplanet Archive: https://exoplanetarchive.ipac.caltech.edu/
- Rein, H. & Liu, S.-F. (2012). *REBOUND: An open-source multi-purpose N-body code*
- Scikit-learn Documentation
- Kepler-90 system discovery and follow-up studies

---

## License

MIT License

---

This project is ideal for research-based coursework, BSc/MSc theses, or hobbyist astrophysics data science exploration.

