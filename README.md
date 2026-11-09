# 🦖 Triceratops Spatial Matrix — Prototype v0.5

An interactive, holographic **6D multi-spectral anatomical engine** for *Triceratops* — spanning a geo globe, 3D skull, whole-body layers, dental battery, bone histology, palaeopathology, growth curves, and population modelling in a single windowed interface.

> ⚠️ **Prototype Sample** — Asia Khan, Hon. BA (McMaster University) · Behavioural UX Researcher & 3D Spatial Architect
> **All Rights Reserved.** Information in this repository is still under review. See [RIGHTS.md](RIGHTS.md) if available, or read the Rights section below.

**🔗 Live Demo:** `https://khan34535-sudo.github.io/Triceratops-Spatial-Matrix/` *(update if your Pages URL differs)*

## 🧭 What This Is

**Triceratops Spatial Matrix** is a browser-based prototype that reimagines how a single extinct animal can be presented as **layered, multi-dimensional data** rather than a single rotating model. It treats *Triceratops* not as one object but as a stack of interacting evidence — spatial, temporal, spectral, chemical, and interpretive — that a viewer can navigate in any order.

The project is a **design and UX research prototype**, not a peer-reviewed scientific resource. It exists to demonstrate a visualisation architecture: how six independent axes (X, Y, Z, T, λ, C) can be applied consistently across wildly different views — a globe, a skull, a tooth, a thin section — without losing coherence. Every window uses the same axis vocabulary, the same band/chemistry controls, and the same evidence-confidence tagging, so a viewer who learns the system once can read any lab in it.

**What it is:**
- A **holographic 6D anatomical engine** — six axes applied uniformly across every viewer.
- A **windowed app shell** — globe as home, every lab as a floating panel with tab bar, pager, and keyboard navigation.
- A **teaching-oriented prototype** — every model is a simplified schematic, labelled as such, with disclaimers visible in the UI.

**What it is not:**
- Not a scan dataset, photogrammetry capture, or museum-grade reconstruction.
- Not a source of measured chemistry, isotope, or population values.
- Not a substitute for the published literature listed in the Notes window.

## 🪟 The Sections, Organised

Each section is a "window" in the app shell. They are arranged so a visitor can move from **where the animal lived** → **what it was** → **how its body worked** → **how we know** → **what we don't know**.

### 1. Where it lived — *Globe*
The entry point and home view. An interactive orthographic globe showing the five key fossil formations (Hell Creek, Lance, Denver, Scollard, Frenchman) and twelve target institutions. Switching from **3D → 6D** progressively adds the Western Interior Seaway (4D), palaeoclimate recolour (5D), and spectral/chemistry overlays (6D). 
**Purpose:** Establish geographic and temporal context before the viewer meets the animal.

### 2. What it was — *Skull*
A rotatable 3D wireframe skull with frill, horns, beak, tooth rows, and inferred brain cavity. Cut plane slices the near side away; the age slider grows the horns and frill in real time; chemistry focus highlights which tissues preserve which signals. 
**Purpose:** Demonstrate how a single axis (age) can transform a model's geometry live, and how "inferred" features (brain cavity) sit visibly alongside "direct" ones (horns).

### 3. How its body worked — *Body*
A holographic SVG side view with seven toggleable layers: skin, skeleton, teeth, vascular flow, organs, health hotspots, and scan sweep. Age slider scales the whole animal; cutaway slider fades the skin; evidence filter dims layers tagged "inferred" vs "direct." 
**Purpose:** Show a body as an assembly of evidence layers, not a single silhouette — and make the inferred/direct distinction a first-class visual control.

### 4. What it ate — *Teeth*
Single-tooth and dental-battery 3D models with a live wear slider. In battery mode, fresh replacement teeth are visible beneath each worn one. 
**Purpose:** Make the dental-battery replacement system — the defining feature of hadrosaur and ceratopsian feeding — legible as a 3D mechanism, not a diagram.

### 5. How we know its age — *Histology*
A procedurally generated thin-section simulator showing LAGs (lines of arrested growth), secondary osteons, primary vascular canals, osteocyte lacunae, and the external fundamental system (EFS). The age slider drives the count of visible LAGs, the amount of internal remodelling, and whether the EFS has formed. Transmitted and polarised light modes. 
**Purpose:** Show the *method* behind age estimates — and why remodelling erases early growth lines, making raw LAG counts underestimate true age.

### 6. What went wrong — *Health*
A palaeopathology table covering bite wounds, combat injuries, fractures, infection-type lesions, cancer, and environmental stress — each tagged **DIRECT**, **PROBABLE**, **CASE-DEPENDENT**, or **RELATIVE ONLY**. 
**Purpose:** Demonstrate honest evidence grading — including the case where a condition is documented only in a relative (*Centrosaurus* osteosarcoma), not in *Triceratops* itself.

### 7. How many existed — *Growth*
An illustrative logistic growth curve with an uncertainty band and an adjustable population model (density, area, lifespan, generation length) following Damuth's-law logic. 
**Purpose:** Show how a population estimate is built from explicit, changeable assumptions — and how sensitive the answer is to those assumptions.

### 8. What we know for sure — *Facts*
Key metrics (length, mass, skull size, temporal range), diet, and the palaeo-osteology methods underlying the labs. 
**Purpose:** Anchor the visualisations in concrete, citable numbers and name the methods (histology, CT, photogrammetry, microwear, isotopes, taphonomy) that the other windows illustrate.

### 9. How to read the system — *Matrix*
A summary table showing how the six axes map across all five main viewers (Globe, Skull, Body, Teeth, Histology). 
**Purpose:** Provide a single reference page so a viewer can see the whole architecture at once — and understand that "X" means longitude on the globe but yaw on the skull, while "T" means 68–66 Ma on the globe but age 0–25 years everywhere else.

### 10. What we're not sure about — *Notes*
Disclaimers and key literature. 
**Purpose:** Make the prototype's limits explicit — illustrative chemistry, stylised geography, simplified anatomy, procedural histology, modelled populations — and point to the published sources that should be used instead for real work.

### 11. Who made it — *Credits*
Prototype label, author, contact links. 
**Purpose:** Attribution and outreach.

## 🎯 Purpose

The prototype serves three overlapping goals:

1. **As a UX research artefact:** To test whether a consistent six-axis vocabulary can hold across radically different data types — map, mesh, SVG, canvas — without becoming confusing. The windowed shell, accordion panels, evidence tags, and live axis readouts are all part of that experiment.
2. **As a teaching aid:** To make visible the *methods* behind palaeontological claims — not just the conclusions. Every window shows its work: the histology lab shows why LAG counts underestimate age; the health table shows why "cancer" is graded *relative only*; the growth window shows how population estimates move when assumptions change.
3. **As a portfolio piece:** To demonstrate a design approach — treating a single subject as layered, navigable, honest data rather than a hero render — applicable to archaeology, palaeontology, museum interpretation, and any domain where evidence comes with confidence levels.

## 🧭 The Six Axes

| Axis | Meaning | Example (Globe / Skull / Body / Teeth / Histology) |
|---|---|---|
| **1 · X** | Primary spatial | Longitude / Yaw / Length / Yaw / Cortex thickness |
| **2 · Y** | Secondary spatial | Latitude / Pitch / Mass / Pitch / Growth lines (LAGs) |
| **3 · Z** | Depth / cut | Zoom / Cut plane / Cutaway / Wear / Remodelled bone |
| **4 · T** | Time | 68–66 Ma / Age 0–25 yrs / Age / Age / Age |
| **5 · λ** | Spectral band | Visible · Thermal · X-ray / CT · UV |
| **6 · C** | Chemistry focus | Hydroxyapatite · Collagen · Keratin · Isotope fidelity |

## ✨ Features

- **Windowed app shell** — globe as home, every other lab opens as a floating panel with tab bar, pager (◀ ▶), dock, and keyboard navigation (← →, Esc).
- **Six-axis readout** across every viewer, updating live as you interact.
- **4D age system** linked across skull, body, teeth, histology, and growth chart.
- **Spectral band filters** (Visible · Thermal · X-ray / CT · UV) applied consistently to 3D viewers, SVG hologram, and histology canvas.
- **Chemistry focus** with tissue-by-tissue relative-value bars.
- **Accordion control panels** — dense information without scrolling overload.
- **Responsive** layout down to mobile; respects `prefers-reduced-motion`.

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Rendering | Vanilla JavaScript · SVG · HTML Canvas 2D |
| Styling | Hand-written CSS (no framework) with CSS custom properties |
| 3D engine | Custom ~150-line projection renderer (no Three.js dependency) |
| Hosting | GitHub Pages (fully static, no backend) |

## 🚀 How to Use

1. Open the **live demo** — the globe loads first as the home view.
2. Click any **dock button** or **tab** to open a lab, or use the **◀ ▶** pager / arrow keys.
3. In the globe, drag to rotate, click markers for formation/institution detail, and switch **3D → 6D** to add time, climate, band, and chemistry.
4. In the 3D labs, drag to rotate, use the sliders for cut plane / wear / age, and switch band and chemistry to highlight tissue types.
5. Press **Esc** or **✕ Back to globe** to return home.

## 📚 Key References

*(Verify before citing — see Notes window)*

- Marsh, O. C. (1889). Notice of gigantic horned Dinosauria from the Cretaceous.
- Horner, J. R., & Goodwin, M. B. (2006). Major cranial changes during *Triceratops* ontogeny. *Proc. R. Soc. B*.
- Farke, A. A., Wolff, E. D. S., & Tanke, D. H. (2009). Evidence of combat in *Triceratops*. *PLoS ONE*.
- Scannella, J. B., & Horner, J. R. (2010). *Torosaurus* Marsh, 1891, is *Triceratops* Marsh, 1889. *J. Vert. Paleo.*
- Longrich, N. R., & Field, D. J. (2012). *Torosaurus* is not *Triceratops*. *PLoS ONE*.
- Horner, J. R., Goodwin, M. B., & Myhrvold, N. (2011). Dinosaur census reveals abundant *Tyrannosaurus*… *PLoS ONE*.
- Ekhtiari, S. et al. (2020). First case of osteosarcoma in a dinosaur. *Lancet Oncology*.
- Marshall, C. R. et al. (2021). Absolute abundance and preservation rate of *Tyrannosaurus rex*. *Science*.

## ⚠️ Disclaimer

- **Chemistry bars are illustrative**, not measured values.
- **Geography is approximate** — land outlines and the Western Interior Seaway are stylised.
- **Anatomy is a simplified teaching model**, not scan data. Vascular, organ, and thermal layers are inferred from living relatives (birds, crocodilians).
- **The bone-histology image is a procedurally generated schematic**, not a real thin section.
- **Population figures come from an adjustable model**, not a measured count.
- **Age, growth, and wear are illustrative models**, not published ontogenetic regressions.

Do not cite figures, overlays, or model outputs as primary data.

## © Rights & Review Status

**Copyright (c) 2026 khan34535-sudo. All Rights Reserved.**

No part of this repository — code, models, SVG assets, data, text, or imagery — may be copied, reproduced, modified, distributed, published, sublicensed, or used commercially without prior written permission from the copyright holder. Viewing the public repository or live demo grants no license.

**Status: UNDER REVIEW** — the information, visualisations, palaeontological interpretations, and modelling assumptions contained in this project are provisional and may be incomplete, inaccurate, or subject to change. This project is **not** a final, authoritative, or peer-reviewed record unless explicitly stated otherwise. Users should not cite, republish, or rely on this material as definitive without independent verification and written permission.

**Contact:** [github.com/khan34535-sudo](https://github.com/khan34535-sudo) · asiaaamirkhan@outlook.com
