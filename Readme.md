# General Stacking Fault Energies of Niobium–Vanadium (Nb–V) Alloys

**AME5970: Computational Materials Science**  
**University of Oklahoma**  
**Instructor:** Dr. Shuozhi Xu  
**Semester:** Spring 2026  

---

## Content Summary

### Project 1

The following alloy compositions are included:

- Nb0.05V0.95
- Nb0.1V0.9
- Nb0.2V0.8
- Nb0.3V0.7
- Nb0.4V0.6

### Project 2

Temperature-dependent simulations were conducted for the following alloy compositions.

#### Nb0.05V0.95

- Nb0.05V0.95 @ 300 K
- Nb0.05V0.95 @ 500 K
- Nb0.05V0.95 @ 900 K
- Nb0.05V0.95 @ 1200 K

#### Nb0.4V0.6

- Nb0.4V0.6 @ 300 K
- Nb0.4V0.6 @ 500 K
- Nb0.4V0.6 @ 900 K
- Nb0.4V0.6 @ 1200 K

## Folder Contents

Each simulation folder contains the following files:

1. `lmp_mcnpt.in`  
   Input file for the Monte Carlo NPT (MCNPT) simulation.

2. `lmp_gsfe.in`  
   GSFE simulation input file.
   - The integer value on **line 54** is set to `10`.

3. `data.CSRO`  
   Data file generated from the CSRO simulation.

4. `log.lammps`  
   Output log file from the CSRO simulation.

5. `gsfe-*` files  
   A total of 20 GSFE output files:
   - `gsfe-1`
   - `gsfe-2`
   - ...
   - `gsfe-20`

   The integer suffix corresponds to the value specified on **line 54** of the associated `lmp_gsfe.in` file.

6. USFE results  
   Files containing:
   - All 20 calculated USFE values
   - Mean USFE value

   Results are provided in either:
   - `.txt`
   - `.xlsx`

## Reference

Simulations and analysis methods are based on:

> Richard Brinlee, Amin Poozesh, Anvesh Nathani, Anshu Raj, Xiang-Guo Li, Iman Ghamarian, Shuozhi Xu,  
> *Integrating atomistic simulations and machine learning to predict unstable stacking fault energies of refractory non-dilute random alloys*,  
> JOM 77 (2025) 8127–8136.
