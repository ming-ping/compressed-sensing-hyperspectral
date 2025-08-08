# Compressed Sensing for Hyperspectral Imaging (CASSI)

This is a personal side project to explore the application of **Compressed Sensing (CS)** to **snapshot hyperspectral imaging** using simulated CASSI (Coded Aperture Snapshot Spectral Imaging) models.

## 🔍 Project Goal

Reconstruct full 3D hyperspectral data cubes from a single or few 2D compressed measurements using sparse priors and CS algorithms.

## 📅 Timeline

12-week plan (Aug–Nov 2025) — ~20 hours/week:
- Forward model simulation
- ℓ1-based sparse recovery
- Dictionary learning or deep CS models
- Realistic noise and reconstruction evaluation

## 📁 Folder Overview

| Folder         | Purpose |
|----------------|---------|
| `data/`        | Hyperspectral image datasets (e.g., from CAVE) |
| `notebooks/`   | Jupyter notebooks for each step |
| `src/`         | Python modules (forward model, CS solver) |
| `results/`     | Output images, plots, metrics |
| `experiments/` | Scripted tests under different conditions |

## 🧪 Technologies Used

- Python, NumPy, OpenCV, Matplotlib
- `cvxpy` for sparse optimization
- `scikit-learn` for dictionary learning
- CAVE Hyperspectral Dataset (31-band images)

## ▶️ How to Run

```bash
# Set up virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run a basic forward + reconstruction test
python experiments/run_baseline.py

📈 Sample Results (To Be Added)
	•	Ground truth vs. reconstructed spectral cubes
	•	PSNR / SSIM comparisons
	•	Effects of noise, mask patterns

🤝 Acknowledgments
	•	Columbia CAVE dataset
	•	Papers on CASSI and compressive imaging

📌 TODOs
	•	Add TV-regularized solver
	•	Simulate realistic optics noise
	•	Benchmark against non-CS recovery

---

## 📦 `requirements.txt`

```txt¯
numpy
scipy
matplotlib
opencv-python
cvxpy
scikit-learn
jupyterlab
h5py
