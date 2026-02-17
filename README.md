# Landscape Carbon Trajectories After Spruce Budworm Outbreaks in Canada’s Eastern Boreal Forest: Effects of Salvage Intensity and Wood-Use Pathways 

## Overview
This project evaluates the role of salvage biomass harvesting as a climate change mitigation strategy in the eastern Canadian boreal forest, particularly following **spruce budworm (SBW)** outbreaks. Using the **LANDIS-II forest landscape model** and its extensions, the study quantifies how directing SBW-killed biomass into **bioenergy** or **harvested wood products (HWP)** affects long-term carbon dynamics and net greenhouse gas emissions under multiple climate change scenarios (Baseline, RCP2.6, RCP4.5, RCP8.5).

## Objectives
- Simulate long-term (2010–2110) ecosystem carbon dynamics in Québec’s Côte-Nord region.  
- Assess salvage biomass scenarios (S0 = reference; S1 = +1000 ha; S2 = +2000 ha; S3 = +4000 ha).  
- Evaluate carbon flows across ecosystem pools, harvested wood products, and operational emissions.  
- Compare utilization pathways (bioenergy vs. sawnwood with 35-year and 60-year half-lives).  
- Estimate **Net Sector Production (NSP)** as an integrative indicator of mitigation potential.

## Methods
- **Modeling framework:**  
  - LANDIS-II v7.1  
  - Extensions: ForCS v3.1, Base Fire, Biomass Harvest, Base BDA (SBW), Base Wind  
- **Study area:** Côte-Nord, Québec (spruce–feathermoss and balsam fir–white birch domains).  
- **Disturbances simulated:** SBW outbreaks, fire, windthrow, and harvesting.  
- **Carbon accounting:** Full supply-chain analysis including harvesting, forwarding, transport (Python KD-tree & networkx shortest path), sawing, chipping, and pelletization.  
- **HWP life cycle:** IPCC Tier 2 decay functions applied to pulp & paper, sawnwood, and bioenergy.  

## Key Findings
- **Ecosystem impacts:** Salvage had limited effect on dead organic matter pools (<2 MtCO₂eq yr⁻¹).  
- **Operational emissions:** Relatively small compared to ecosystem fluxes; dominated by pelletization (~0.15 MtCO₂eq yr⁻¹).  
- **HWP outcomes:**  
  - Bioenergy → net carbon debt due to immediate emissions.  
  - Sawnwood (35 yr) → modest storage, but decomposition outweighed benefits.  
  - Sawnwood (60 yr) → doubled storage, reduced emissions, and generated **net carbon credits** under RCP4.5–RCP8.5 by late century.  
- **Overall:** Climate benefits of salvage harvesting are **highly dependent on product type and longevity**. Substitution effects (not modeled here) would likely increase the benefits.

## Requirements
- **LANDIS-II v7.1** with extensions (ForCS v3.1, BDA, Fire, Wind, Harvest).  
- **R (≥4.0)** with packages: `ggplot2`, `data.table`, `patchwork`, `dplyr`.  
- **Python (≥3.9)** with `numpy`, `scipy`, `networkx`, `pandas`.  

## Authors
- **A. Ameray**, **D.S. Pureswaran**, **J. Laganière**, **R.W. Buchkowski**  
- Canadian Forest Service, University of Western Ontario, Groupe Canalytics




