# 🚀 1D Rocket Flight Simulator & Motor Thrust Analyzer

A Python-based simulation engine and data processing toolkit designed to convert static test-stand thrust data into continuous mathematical models, compute total impulse, and run numerical 1D 4th-order Runge-Kutta (RK4) trajectory simulations.

---

## 📖 Live API Documentation

Explore the full, interactive function-level reference and docstrings hosted via GitHub Pages:
👉 **[View the Live API Documentation](https://atur0021.github.io/MMA3001-Project/Flight_Simulator_Documentation.html)**

---

## ✨ Features

- **Dynamic Thrust Processing:** Automatically detects motor ignition spikes, calculates baseline sensor offsets, compensates for liquid oxidizer mass depletion over time, and crops active thrust windows.
- **Noise Filtering & Spline Fitting:** Fits smooth `UnivariateSpline` curves through noisy raw thrust sensor data and evaluates fit quality (R^2).
- **Impulse Integration:** Computes integrated total motor impulse using Simpson's 1/3 rule.
- **RK4 Flight Simulation:** Solves 1D rocket dynamic equations of motion considering variable vehicle mass, atmospheric density models (US Standard Atmosphere), and aerodynamic drag forces. Generates plots for altitude, velocity, acceleration, and mass depletion curves.

---

## 📁 Repository Structure

```text
.
├── data/
│   └──                                      # Contains raw thrust curve data, raw flight data, and cleaned flight data
├── docs/
│   └── Flight_Simulator_Documentation.html  # Generated pdoc API documentation
├── Flight_Data_Extractor.ipynb              # Secondary notebook used for cleaning raw flight data
├── MMA3001-Project.ipynb                    # Primary notebook for performing the simulation
└── README.md                                # Project overview
