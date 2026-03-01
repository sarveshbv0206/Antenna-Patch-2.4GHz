# 2.45 GHz Microstrip Patch Antenna on FR4

This repository presents the design, simulation, optimization, and validation of a
**2.45 GHz inset-fed rectangular microstrip patch antenna** using **CST Studio Suite**.

The focus of this project is correct RF design methodology rather than blind optimization.

---

## Specifications

| Parameter | Value |
|---------|------|
| Operating frequency | 2.45 GHz |
| Frequency sweep | 2.2 – 2.6 GHz |
| Antenna type | Rectangular microstrip patch |
| Substrate | FR4 (lossy) |
| Relative permittivity (εr) | 4.3 |
| Substrate thickness | 1.6 mm |
| Substrate size | 39 × 47 mm |
| Feed type | Inset microstrip feed |
| Solver | CST Time Domain |

---

## Design Methodology

Initial dimensions were calculated using standard microstrip antenna equations.
Due to dielectric losses, fringing fields, and finite ground size, analytical values
were used only as a starting point.

The design was refined using parametric sweeps.

---

## Optimization Strategy

1. **Patch length sweep**
   - Purpose: Resonant frequency tuning
2. **Inset feed length sweep**
   - Purpose: Impedance matching

Patch length was optimized first, followed by inset feed depth.
This avoids incorrect matching-based tuning.

---

## Final Optimized Dimensions

| Parameter | Value |
|---------|------|
| Patch length | 28.6 mm |
| Patch width | 37.2 mm |
| Inset depth | 6.0 mm |
| Feed width | ~3.1 mm |

---

## Results

- S11 ≈ −22.8 dB @ 2.46 GHz  
- VSWR ≈ 1.24 @ 2.45 GHz  
- Peak realized gain ≈ 1.73 dBi  
- Broadside radiation pattern  

Reduced gain is expected due to FR4 dielectric losses and compact substrate size.

---

## Field Distribution

- **E-field:** Concentrated at patch edges, confirming fringing-field radiation
- **H-field:** Concentrated beneath the patch and near feed line, indicating proper current flow

---

## Tools Used

- CST Studio Suite (Time Domain Solver)

---

## Author

Sarvesh B. V.  
B.E. Electronics & Communication (Advanced Communication Technology) 

---

## Notes

This project demonstrates correct RF antenna design workflow rather than aggressive
numerical optimization.
