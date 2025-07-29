# QHS–LIGO Template Matching: Gravitational Analog Detection from Vortex Dynamics

This repository contains code and data for matched filtering of **Quantum Harmonic Shift (QHS)**-derived waveforms against gravitational wave templates using the [PyCBC](https://pycbc.org) library. The goal is to test for structural similarity between QHS-emergent gravitational analogs and templates used by LIGO.

---

## 📂 Contents

- `mass_sweep_qhs.py` — Main script for whitening, filtering, and matched filtering using a grid sweep over GR template parameters.
- `qhs_waveform_normalized.csv` — Normalized strain data from QHS simulations (input waveform).
- `requirements.txt` — Python dependencies.
- `results/` — Output folder for SNR heatmaps and matched parameters (you create this).
- `README.md` — Project overview.

---

## 🧪 Objective

To validate the hypothesis that **spin-2 gravitational wave analogs** emerge from scalar vortex dynamics, this pipeline:

1. Loads a QHS-derived waveform (strain vs. time)
2. Applies whitening and highpass filtering
3. Sweeps through mass parameters for binary black hole mergers (GR templates)
4. Computes matched filter signal-to-noise ratio (SNR)
5. Visualizes results via a heatmap and outputs best-fitting parameters

---

## 🛠️ Installation

To run this analysis:

1. **Clone the repo**
   ```bash
   git clone https://github.com/YOUR_USERNAME/QHS_LIGO_MatchedFiltering.git
   cd QHS_LIGO_MatchedFiltering
