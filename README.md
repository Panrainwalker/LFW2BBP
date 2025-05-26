# LFW2BBP: Broadband Ground-Motion Parameters Estimation Using Physics-Based Simulated Low-frequency Waveforms and Deep Learning

Accurate prediction of broadband ground motion parameters is crucial for earthquake disaster prevention and mitigation. However, physics-based ground motion simulations are limited by the lack of high-wavenumber components in source rupture models and velocity structures, making them reliable only for low-frequency ground motions (typically <1 Hz).

To address this limitation, we propose **LFW2BBP**, a deep learning framework designed to map low-frequency physics-based simulated ground motion waveforms to broadband ground motion parameters.

## 🧠 Overview

**LFW2BBP** leverages multiple domain features of low-frequency waveforms:

- **Time-domain waveforms**
- **Time-frequency signals**
- **Spectral acceleration**

These features are jointly encoded and used to predict key broadband parameters such as PGA (Peak Ground Acceleration), PGV (Peak Ground Velocity), SA (Spectral Acceleration) at multiple periods.

## 🧪 Key Features

- **Physics-based**: Uses physics-based simulated low-frequency data as input.
- **Multi-domain inputs**: Combines waveform, spectral, and spectral acceleration features.
- **Validated**: Tested against observed data from the 2016 $M_w$ 7.0 Kumamoto earthquake.

## 📁 Project Structure

```plaintext
LFW2BBP/
├── LF_sim_data/                      # Low-frequency simulation data for 2016 Kumamoto
├── models/                           # Trained model weights
├── evaluate_kumamoto_sim_05Hz.ipynb  # Evaluation notebook for Kumamoto earthquake
└── README.md                         # Project documentation
```

---
## Install dependencies:
```bash
pip install -r requirements.txt
