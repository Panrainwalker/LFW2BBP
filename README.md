# LFW2BBP: Learning-Based Mapping from Low-Frequency Simulation to Broadband Parameters

Accurate prediction of broadband ground motion parameters is crucial for earthquake disaster prevention and mitigation. However, physics-based ground motion simulations are limited by the lack of high-wavenumber components in source rupture models and velocity structures, making them reliable only for low-frequency ground motions (typically <1 Hz).

To address this limitation, we propose **LFW2BBP**, a deep learning framework designed to map low-frequency physics-based simulated ground motion waveforms to broadband ground motion parameters.

## 🧠 Overview

**LFW2BBP** leverages multiple domain features of low-frequency waveforms:

- **Time-domain waveforms**
- **Time-frequency spectra**
- **Spectral acceleration (SA)**

These features are jointly encoded and used to predict key broadband parameters such as PGA (Peak Ground Acceleration), PGV (Peak Ground Velocity), SA at multiple periods, and duration metrics.

## 🧪 Key Features

- **Physics-aware**: Uses physically simulated low-frequency data as input.
- **Multi-domain learning**: Combines waveform, spectral, and acceleration features.
- **Generalizable**: Shows robustness to data variability through sensitivity testing.
- **Validated**: Tested against observed data from the 2016 $M_w$ 7.0 Kumamoto earthquake.

## 📁 Project Structure
LFW2BBP/
│
├── LF_sim_data/ # Low-frequency simulation input
├── models/ # Trained model weights (e.g., best_model_05.pth)
├── notebooks/ # Jupyter notebooks for analysis
├── utils/ # Supporting utility scripts
├── 4evaluate_kumamoto_sim_05Hz.ipynb # Evaluation notebook
└── README.md


Install dependencies:
```bash
pip install -r requirements.txt
