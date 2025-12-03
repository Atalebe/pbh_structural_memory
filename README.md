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
├── README.md
├── LICENSE
├── CITATION.cff           # optional
├── environment.yml        # or requirements.txt
├── paper/
│   ├── main.tex           # LaTeX source (Scientific Reports / A&A style)
│   ├── pbh_bounce.bib     # bibliography
│   ├── fig1.pdf           # PBH survival window
│   ├── fig2.pdf           # SMBH seed growth tracks
│   ├── fig3.pdf           # schematic dual–component mass function
│   └── fig_anisotropy.pdf # schematic PBH dipole-like modulation
├── figs/
│   ├── alignment_threshold_curve.png       # PBH–CMB alignment sensitivity
│   ├── mass_function_discrimination.png    # mass–function detection probability
│   └── fig_anisotropy.png                  # illustrative anisotropy sky
└── code/
    └── pbh_alignment_test/
        ├── run_alignment_scan.py           # PBH–CMB alignment Monte Carlo
        ├── run_mass_function_sim.py        # mass–function Bayes factor forecast
        ├── run_gw_anisotropy_proj.py       # GW projection–statistic forecast
        ├── run_gw_anisotropy_sim.py        # (optional) earlier GW estimator
        └── make_fig_anisotropy.py          # generates fig_anisotropy.* files
