# MATLAB-Based Numerical Simulation of BCR-ABL1 Dynamics in Chronic Myeloid Leukemia

This project simulates BCR-ABL1 mRNA and protein/activity dynamics in Chronic Myeloid Leukemia (CML) using MATLAB and numerical analysis methods.

The model compares:

* Normal cells
* Untreated CML cells
* Treated CML cells under TKI inhibition

The project was developed as part of a Numerical Analysis / MATLAB course project.

---

## Methods Used

* Euler Method
* MATLAB `ode45`
* ODE-based biological modeling

---

## Model Equations

### mRNA dynamics

[{dM}/{dt} = k_m - d_m M]

### Protein/activity dynamics

[{dP}/{dt} = k_p M - d_p P - uP]

Where:

* `M` = BCR-ABL1 mRNA level
* `P` = BCR-ABL1 protein/activity level
* `u` = treatment inhibition strength

---

## Simulation Parameters

The Euler Method and `ode45` simulations were performed using manually selected parameter values to represent different biological conditions.

Different parameter sets were used for:

* Normal cells
* Untreated CML cells
* Treated CML cells

The parameters were chosen for educational and simulation purposes to demonstrate how changes in transcription, degradation, and treatment inhibition affect BCR-ABL1 activity dynamics.

---

## GEO Dataset Analysis

This project also includes a simple transcriptomic analysis using the GEO dataset:

`GSE33075`

The GEO analysis was used to check whether gene expression levels decrease after treatment, and to compare the biological trend with the simulation results.

Before running the GEO analysis section:

1. Search for the GEO dataset using the accession ID:
   `GSE33075`

2. Download:
   `GSE33075_series_matrix.txt.gz`

3. Extract the file before running the MATLAB scripts.

Dataset link:
https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE33075

## What the simulation shows

* Higher BCR-ABL1 activity in untreated CML
* Reduced activity after treatment inhibition
* Similar trends between Euler Method and MATLAB ode45
* Reduced activity with stronger inhibition values

The GEO transcriptomic analysis also showed reduced gene expression after treatment, supporting the expected simulation behavior.

## Tools:
* MATLAB
* Numerical Analysis
* ODE Simulation
* Computational Biology

