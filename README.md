# pbh_structural_memory
Simulation code and figure-generation scripts for "Anisotropic primordial black holes as a fossil record from a pre-Big Bang universe." Paper
# Anisotropic primordial black holes as a fossil record from a pre-Big Bang universe

This repository contains the LaTeX source, simulation code, and derived figures
for the manuscript:

> **Anisotropic primordial black holes as a fossil record from a pre-Big Bang universe**  
> Stephen Atalebe (Masaryk University, Brno, Czech Republic)

The paper explores a conservative but testable scenario in which a subset of
primordial black holes (PBHs) survive a finite–density cosmological bounce and
carry **structural memory** from a pre–Big Bang phase. This survival–weighted
PBH population generates:

- a few–percent anisotropy aligned with the CMB quadrupole–octopole axis,
- a dual–component PBH mass function (log–normal + power–law tail),
- an enhanced population of 30–50 M☉ mergers in gravitational–wave catalogues.

The repository includes the Monte Carlo forecasts for:

1. **PBH–CMB alignment sensitivity** (Fig. 4 in the paper),
2. **Mass–function discrimination** (dual–component vs single log–normal),
3. **Gravitational–wave anisotropy** with realistic localisation errors.

---

## Repository structure

```text
pbh_structural_memory/
 ├── paper/
 │    ├── main.tex
 │    ├── pbh_bounce.bib
 │    ├── all_figures/
 │    │      ├── alignment_threshold_curve.png
 │    │      ├── mass_function_discrimination.png
 │    │      ├── fig_anisotropy.png
 │    │      ├── fig_anisotropy.pdf
 │    │      ├── fig1.pdf
 │    │      ├── fig2.pdf
 │    │      ├── fig3.pdf
 │    │      ├── fig_survival.pdf
 │    │      ├── fig_smbh_growth.pdf
 │    │      ├── fig_mass_function.pdf
 │    │      └── (any others)
 │    └── (anything else needed for LaTeX compile)
 ├── simulations/
 │    ├── run_alignment_threshold.py
 │    ├── run_mass_function_sim.py
 │    ├── run_gw_anisotropy_proj.py
 │    ├── make_fig_anisotropy.py
 │    ├── utils/
 │    │     ├── anisotropy_tools.py
 │    │     └── mass_tools.py
 │    └── outputs/
 │          ├── alignment_threshold_curve.png
 │          ├── mass_function_discrimination.png
 │          └── fig_anisotropy.png
 └── README.md
