# ML-Based Exoplanet Atmosphere Inference

This project aims to leverage Machine Learning (ML), especially Deep Learning, to detect and analyze atmospheric components of exoplanets from transmission spectroscopy data. The goal is to create a publishable research piece aligned with ongoing academic efforts in top US universities.

---

## Project Roadmap

### Month 1 – Background & Setup

#### Step 1: Understand the Problem
- Study spectroscopy techniques used to study exoplanet atmospheres.
- Learn about molecular absorption features in infrared spectra (e.g., H₂O, CO₂, CH₄).
- Understand transit spectroscopy (transmission spectra) and how it works.

#### Step 2: Learn the Tools
Learn Python libraries:
- `numpy`, `matplotlib`, `pandas`
- `scikit-learn`, `tensorflow` or `pytorch`
- `astropy`, `lightkurve`, `petitRADTRANS`

Review ML concepts:
- Supervised learning
- Neural networks (especially CNNs)
- Overfitting and model evaluation techniques

#### Step 3: Research Alignment
- Review recent papers from:
  - University of Arizona
  - University of California, Santa Cruz (OWL Lab)
  - Arizona State University
- Identify datasets, models, and spectral features used in current research.

---

### Month 2 – Data Collection & Preparation

#### Step 4: Gather Datasets
- Generate simulated spectra using:
  - `petitRADTRANS`
  - `ExoGAN`
- Collect real spectra from:
  - NASA Exoplanet Archive
  - MAST (Mikulski Archive)
  - JWST Early Release Science datasets

#### Step 5: Preprocess Data
- Clean and normalize spectral data.
- Label each spectrum with known atmospheric components.
- Split the dataset: 70% training, 15% validation, 15% test.

---

### Month 3 – Model Development

#### Step 6: Baseline Model
- Build a basic ML model using:
  - `RandomForestClassifier`
  - Simple MLP (Multi-Layer Perceptron)
- Start with synthetic data.

#### Step 7: Deep Learning Model
- Implement a 1D CNN:
  - Input: normalized spectra (wavelength vs intensity)
  - Output: probability of molecule presence (multi-label classification)
- Use regularization techniques:
  - Dropout layers
  - Data augmentation (add noise)

#### Step 8: Evaluate & Tune
- Evaluate model using:
  - Precision/Recall per molecule
  - ROC-AUC scores
  - Confusion matrix
- Perform hyperparameter tuning:
  - Learning rate, batch size, epochs, layer configuration

---

### Month 4 – Real Data Testing + Explainability

#### Step 9: Apply to Real Data
- Test the model on real-world spectra (e.g., from Hubble or JWST).
- Compare model output with published molecular detections.
- Look for novel predictions or confirmations.

#### Step 10: Model Explainability
- Use `SHAP` or `LIME` to analyze:
  - Which spectral features influence the predictions.
- Visualize importance of wavelength regions per molecule.

---

### Month 5 – Documentation & Results

#### Step 11: Analysis
- Document performance metrics and results.
- Highlight novel findings or insights from your model.
- Identify any areas where the ML model improves over traditional methods.

#### Step 12: Write Research Paper
- Format the paper in IEEE or AAS style.
- Suggested structure:
  - Abstract
  - Introduction
  - Related Work
  - Data
  - Methodology
  - Results
  - Discussion
  - Conclusion
- Include visuals:
  - Spectra examples
  - Model diagrams
  - Performance plots

---

### Month 6 – Publication & Outreach

#### Step 13: Submit Paper
Target Journals:
- Astrophysical Journal (ApJ)
- Machine Learning: Science and Technology
- Research Notes of the AAS

#### Step 14: Outreach to Professors
- Share your GitHub repo and a 1-page summary with faculty from:
  - University of Arizona
  - UC Santa Cruz
  - Arizona State University
- Ask for feedback or potential collaboration.
- Express interest in MSc programs and research assistantship opportunities.

---

## Technologies and Libraries

| Area         | Tools |
|--------------|-------|
| ML           | TensorFlow, PyTorch, scikit-learn |
| Astronomy    | Astropy, Lightkurve, petitRADTRANS |
| Visualization| Matplotlib, Seaborn, SHAP, LIME |
| Data Sources | NASA Exoplanet Archive, MAST, JWST ERS |
| Documenting  | Overleaf (LaTeX), Jupyter Notebooks, GitHub |

---

## Contact

For collaboration, mentorship, or MSc application-related queries, feel free to reach out via email or GitHub.

