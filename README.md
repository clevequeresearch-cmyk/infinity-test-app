# Infinity Test Nomogram

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17718092.svg)](https://doi.org/10.5281/zenodo.17718092)

Field-based web application to estimate **VO₂∞**, **equivalent power** and **maximal aerobic speed (MAS)** from a 3-minute all-out wheelchair *Infinity Test*.

- 🔬 Designed for manual wheelchair users (primarily chronic paraplegia)
- 📈 Validated against VO₂peak obtained from arm-crank ergometry
- 📱 Mobile- and tablet-friendly interface
- 📄 One-click **PDF report** export with logo, nomogram and training zones

Live app (GitHub Pages):  
👉 https://clevequeresearch-cmyk.github.io/infinity-test-app/

Archived, citable version (Zenodo):  
👉 https://doi.org/10.5281/zenodo.17718092

---

## Features

- **Automatic computation of laps·min⁻¹**
  - User enters total laps and test duration (default 180 s)
  - Laps per minute is computed and can be fine-tuned if needed

- **VO₂∞ prediction nomogram**
  - Linear model: VO₂∞ (mL·min⁻¹) = 461 × laps·min⁻¹  
  - 95% confidence interval band (grey)
  - Fitness zones based on VO₂∞ in mL·kg⁻¹·min⁻¹ (very low / low–moderate / good–excellent)

- **Equivalent power and MAS**
  - Conversion to VO₂Ergo and equivalent power (W)
  - MAS expressed in m·s⁻¹ and km·h⁻¹
  - MAS-based training zones (≈90%, 100%, ≥110% MAS)

- **Infinity Test lap-counting rules**
  - Figure-eight track with standard lap distance (e.g. 24.4 m)
  - If the athlete completes **more than half** of a final lap, it is rounded **up** to the next full lap
  - If less than or equal to half a lap is completed, it is rounded **down**
  - These rules are displayed in the set-up section of the app

- **Automated PDF reporting**
  - Printable individual report including:
    - Input parameters
    - Predicted VO₂∞, CI and zones
    - MAS and equivalent power
    - Nomogram with current input
    - Infinity Test schematic
    - Software DOI (Zenodo) and QR code

---

## Usage

1. Open the app in a web browser  
   - Online: https://clevequeresearch-cmyk.github.io/infinity-test-app/  
   - Offline: open `index.html` locally (fully standalone).

2. In the **Inputs** panel:
   - Enter the **total laps completed** during the 3-min Infinity Test
   - Enter the **test duration** (default 180 s; adjust if the test was stopped earlier)
   - Check the automatically computed **laps per minute** and adjust if needed
   - Enter **body mass (kg)** and **lap distance (m)**

3. Read the **Individual results** and **MAS-based training zones**.

4. Scroll down to see the full **Infinity Test set-up schematic** and methodological notes.

5. Use the **“Export PDF report”** button to generate a printable report for the athlete, coach or clinician.

---

## Citation

If you use the Infinity Test Nomogram in a scientific publication, please cite:

> Leveque C. *Infinity Test Nomogram – Version 1* (V1.0) [Software]. Zenodo; 2025.  
> DOI: 10.5281/zenodo.17718092

BibTeX:

```bibtex
@software{infinitytest_v1_1,
  author       = {clevequeresearch-cmyk},
  title        = {Infinity Test Nomogram — Version 1.1 (DOI + QR code update)},
  month        = nov,
  year         = 2025,
  publisher    = {Zenodo},
  version      = {v1.1},
  doi          = {10.5281/zenodo.17718602},
  url          = {https://doi.org/10.5281/zenodo.17718602}
}
