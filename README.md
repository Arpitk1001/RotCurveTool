# GRC Fitting Tool

A streamlined Python-based framework for simulating and fitting galactic rotation curves using physically motivated mass models and statistically rigorous inference techniques.

---

## 🚀 Overview

This tool allows researchers to fit observed galactic rotation curves using a combination of bulge, disk, and dark matter halo profiles. It supports tabulated and raw FITS data, multiple halo and bulge models, and offers robust fitting methods including MCMC with full uncertainty propagation.

✅ Reproduces published Milky Way models  
✅ Supports component-wise plotting and residual diagnostics  
✅ Easy to extend, use, and interpret — ideal for both research and teaching

---

## 📦 Features

- Bulge profiles: Hernquist, de Vaucouleurs
- Disk: Exponential disk
- Halo profiles: NFW, Burkert
- Input formats: tabulated data or raw FITS velocity maps
- Fitting methods:
  - Non-linear least squares (`scipy.curve_fit`)
  - Bootstrap resampling
  - Markov Chain Monte Carlo (via `emcee`)
- Output:
  - Rotation curve plot with 1σ band
  - Component decomposition
  - Residual plot
  - MCMC corner plot
  - Reduced χ² and R² goodness-of-fit metrics

---

## 📝 Requirements

Install dependencies using:

```bash
pip install -r requirements.txt
```

---

## 📂 File Structure

```
.
├── RotCurveTool.ipynb      # Main interactive notebook
├── requirements.txt            # Python dependencies
├── rotation_curve_fit.png      # Sample output: total fit
├── residuals_plot.png          # Sample output: residuals
├── mcmc_corner_plot.png        # Sample output: MCMC corner plot
```

---

## 🧪 Quick Start

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/GRC-Fitting-Tool.git
    cd GRC-Fitting-Tool
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Launch the notebook:
    ```bash
    jupyter notebook grc_fitting_demo.ipynb
    ```

---

## 📊 Example Galaxy

The included notebook demonstrates fitting the Milky Way's rotation curve using:
- de Vaucouleurs bulge
- Exponential disk
- NFW halo
- MCMC inference

Data is sourced from Dr. Yoshiaki Sofue’s public rotation curve repository at the University of Tokyo.

---

## 📖 Citation

If you use this tool in your work, please cite:

> Kottur, A. et al. (2025). *A Streamlined Framework for Simulating and Fitting Galactic Rotation Curves*. arXiv:XXXX.XXXXX

---

## 📘 License

This project is licensed under the MIT License — see the `LICENSE` file for details.

---

## 🤝 Acknowledgements

Developed as part of an undergraduate research initiative in galaxy dynamics and dark matter modeling. Inspired by published models by Dr. Yoshiaki Sofue (2016) and community feedback on fitting limitations in tools like RotCur and GalRotPy.
