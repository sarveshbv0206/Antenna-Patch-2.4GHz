# Final Antenna Dimensions

This document lists the final optimized dimensions of the
2.45 GHz microstrip patch antenna as used in the CST simulation.

These values represent the final design after analytical estimation
and parametric optimization.

---

## Substrate Parameters

| Parameter | Value |
|---------|------|
| Substrate material | FR4 (lossy) |
| Relative permittivity (εr) | 4.3 |
| Substrate thickness | 1.6 mm |
| Substrate size | 39 × 47 mm |

---

## Patch Geometry

| Parameter | Value |
|---------|------|
| Patch length (L) | **28.6 mm** |
| Patch width (W) | **37.2 mm** |
| Copper thickness | 0.035 mm |

---

## Feed Parameters

| Parameter | Value |
|---------|------|
| Feed type | Inset microstrip feed |
| Feed width | ~3.1 mm |
| Inset feed length | **6.0 mm** |
| Port impedance | 50 Ω |

---

## Simulation Settings

| Parameter | Value |
|---------|------|
| Solver | CST Time Domain |
| Frequency sweep | 2.2 – 2.6 GHz |
| Boundary conditions | Open (add space) |

---

## Notes

- All dimensions are in millimeters unless stated otherwise.
- Final values were selected based on resonance alignment and impedance matching.
- Small frequency offsets are expected due to FR4 dielectric tolerance.
