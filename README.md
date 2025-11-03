## ⚡ AES Indiana Grid Load Prrof of concept

This repository presents a reproducible **short-term electricity load forecasting** workflow built to mirror the operational challenges faced by **AES Indiana** and other utilities. Using open MISO regional load data as a public proxy for AES’s grid demand, the notebook demonstrates an end-to-end process—data cleaning, feature engineering, baseline ARIMA modeling, and visual forecasting—implemented entirely in Python.

The goal is to provide a transparent, extendable foundation for future utility analytics work, enabling integration with internal AES data sources (SCADA, AMI, weather feeds) and more advanced forecasting techniques such as SARIMA, Prophet, or gradient-boosted models. All results are reproducible in a single Jupyter environment and export ready for dashboards or Power BI integration.

## 🧱 Repository Structure
utility-grid-forecasting/
│
├── 📂 data/
│ ├── 📁 raw/ → Source data (open MISO or synthetic AES proxy data)
│ ├── 📁 processed/ → Cleaned intermediate data (optional)
│ └── 📁 outputs/ → Forecast CSV exports and tables
│
├── 📂 figures/ → Saved visualizations (trends, forecasts, etc.)
│
├── 📂 notebooks/
│ └── utility_grid_forecasting.ipynb → Main Jupyter notebook
│
├── 📄 requirements.txt → Python dependencies
├── 📄 README.md → Project overview and documentation
└── 📄 .gitignore → Ignore patterns for temporary and large files
<img width="468" height="326" alt="image" src="https://github.com/user-attachments/assets/b05e2bbd-4436-4792-9754-c9f3c59841e5" />

Key Deliverables in This Repo
•	Goal: Predict short-term utility grid load (daily/weekly) using open or synthetic data.
•	Core Models: ARIMA → SARIMA → RandomForestRegressor (optional).
•	Visualization: Matplotlib / Plotly (interactive dashboard).

## ⚙️ How to Run

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/<your-username>/utility-grid-forecasting.git
cd utility-grid-forecasting

2️⃣ Set Up the Environment
conda create -n utility python=3.11 -y
conda activate utility
pip install -r requirements.txt

3️⃣ Launch Jupyter Lab
jupyter lab

4️⃣ Open the Notebook
In Jupyter Lab, open: notebooks/utility_grid_forecasting.ipynb

5️⃣ Outputs

Forecast figures are saved to figures/
Forecast CSVs are saved to data/outputs/

## ⚖️ License and Attribution

This project is licensed under the **MIT License** — you are free to use, modify, and distribute this software for any purpose, provided that proper credit is given.

### MIT License

Copyright (c) 2025 Michael S. Mohle

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

