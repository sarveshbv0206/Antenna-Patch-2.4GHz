# Microstrip Patch Antenna Design Equations

This section documents the analytical equations used to estimate the initial
dimensions of the 2.45 GHz rectangular microstrip patch antenna.
These equations provide starting values only; final dimensions were obtained
through simulation-based optimization in CST.

---

## Design Parameters

- Target frequency (f): 2.45 GHz
- Substrate: FR4 (lossy)
- Relative permittivity (εr): 4.3
- Substrate thickness (h): 1.6 mm
- Speed of light (c): 3 × 10⁸ m/s

---

## Patch Width (W)

The patch width primarily affects radiation efficiency and bandwidth.

W = c / (2f) · √(2 / (εr + 1))

For the given parameters:

W ≈ 37.2 mm

---

## Effective Dielectric Constant (ε_eff)

Due to fringing fields, the effective dielectric constant is lower than εr.

ε_eff = (εr + 1)/2 + (εr − 1)/2 · (1 + 12h/W)^(-1/2)

For this design:

ε_eff ≈ 3.9 – 4.0

---

## Length Extension Due to Fringing (ΔL)

Fringing fields at the patch edges increase the effective electrical length.

ΔL = 0.412h · ((ε_eff + 0.3)(W/h + 0.264)) / ((ε_eff − 0.258)(W/h + 0.8))

ΔL ≈ 0.7 mm

---

## Patch Length (L)

The effective resonant length is approximately half the guided wavelength.

L = c / (2f√ε_eff) − 2ΔL

Initial calculated length:

L ≈ 29 mm

---

## Practical Notes

- Analytical equations do not account for dielectric loss, finite ground plane,
  or feed effects.
- FR4 substrate tolerance can introduce frequency shifts of tens of MHz.
- Final patch length was optimized using parametric sweeps in CST.

The final optimized patch length differs slightly from the analytical value.
