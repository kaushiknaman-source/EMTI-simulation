# Naman Kaushik — Portfolio

My portfolio website, plus the code behind its EMTI Lab.

- `index.html` — the whole site in one static file (no build step). Includes the interactive EMTI Lab, where all five simulations run live in the browser.
- `emti/` — the original Python simulations for 21ECC205T Electromagnetic Theory & Interference (LLT-1), with the plot each one produces.

## EMTI simulations

| Script | Topic |
| --- | --- |
| `emti/sim1_gauss_flux.py` | Gauss's law: numerical flux through spherical surfaces |
| `emti/sim2_displacement_current.py` | Displacement current in a parallel-plate capacitor |
| `emti/sim3_lossy_tline.py` | Attenuation and phase on a lossy transmission line |
| `emti/sim4_quarter_wave.py` | Quarter-wave transformer matching 100 Ω to 50 Ω |
| `emti/sim5_smith_chart.py` | Smith chart analysis of a 75 + j25 Ω load |

Run them with Python 3:

```
pip install numpy matplotlib
cd emti
python sim1_gauss_flux.py
```

Each script prints its results and saves its `.png` plot.

## Deploy

Import this repo into Vercel (Framework preset: Other) and deploy. Every push to `main` redeploys the site.
