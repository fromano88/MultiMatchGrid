# Supplementary Material for *Multiscale Modelling of Weakly Porous Grid Flows*

This repository hosts the supplementary PDF accompanying the 2026 doctoral thesis *Multiscale Modelling of Weakly Porous Grid Flows* by **Hossameldin Abdelaziz**. The research was supervised by **Francesco Romanò** at the Laboratoire de Mécanique des Fluides de Lille (LMFL), Arts et Métiers Institute of Technology, Lille, France.

**[Read the supplementary PDF](Supplementary_Material_Detailed_Appendices.pdf)**

The PDF provides numerical methods, spectral results, machine-learning validation, and detailed model comparisons that support the main thesis. It contains four appendices:

## Contents

### A. Numerical implementation of the Uni-Directional Model

This appendix describes the two-dimensional Poisson problem used to approximate axial velocity through a grid aperture. It gives the governing equation and flux normalization, then explains the custom OpenFOAM solver, discretization, linear solver, and convergence criterion.

### B. Spectral analysis and reconstruction errors

This appendix examines the Fourier structure of geometry-resolved square regular grid (SRG) flows. It defines the transverse discrete Fourier transform, modal energy, and inverse reconstruction. Figures show velocity coefficients across porosities and Reynolds numbers. Further comparisons assess truncated reconstructions of the velocity field and streamwise forcing against the geometry-resolved results.

### C. Machine-learning validation of Fourier coefficients

This appendix documents the neural-network models used to predict retained Fourier coefficients from downstream position, porosity, and Reynolds number. It compares predicted and reference coefficients within the training parameter range and at the Reynolds-number extrapolation case Re_H = 100. Training and validation histories are included. The discussion identifies limitations where the reference flow becomes weakly unsteady or departs from the symmetries imposed on the models.

### D. Validation of the velocity-corrected Darcy–Forchheimer model

This appendix provides case-by-case comparisons between geometry-resolved small-scale flow (SSF) and the velocity-corrected Darcy–Forchheimer model (VCDFM). The comparisons cover streamwise evolution, downstream flow patterns, velocity profiles, and transverse planes. They show the model's effective range and its breakdown for selected porosities and Reynolds numbers. The appendix also compares forcing obtained directly from SSF, reconstructed from truncated Fourier modes, and predicted using machine learning.

## Abbreviations

- **UDM:** Uni-Directional Model
- **SSF:** geometry-resolved small-scale flow
- **SRG:** square regular grid
- **TIDFT:** truncated inverse discrete Fourier transform
- **VCDFM:** velocity-corrected Darcy–Forchheimer model

## Acknowledgements

This research was supported by the **French National Research Agency (ANR)** through the *MultiMatchGrid* project (SIREPA 1462). Computational resources were provided by **GENCI–TGCC** under allocation **A0162A01741** and by the **Cassiopée** high-performance computing facility.
