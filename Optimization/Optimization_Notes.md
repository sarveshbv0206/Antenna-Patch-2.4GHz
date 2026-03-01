# Optimization Notes

This section documents the simulation-based optimization process used to
refine the antenna dimensions after analytical design.

The goal of optimization was to:
- Align the resonant frequency with 2.45 GHz
- Achieve good impedance matching (low S11 and VSWR)

---

## Optimization Strategy

Optimization was carried out in a controlled and sequential manner to avoid
misleading results.

Order of optimization:
1. Patch length (frequency control)
2. Inset feed length (impedance matching)

Only one parameter was varied at a time.

---

## Patch Length Optimization

The initial patch length obtained from analytical equations produced resonance
below the target frequency.

A parametric sweep was performed on patch length over a limited range.

Observations:
- Increasing patch length shifted the resonant frequency downward
- Decreasing patch length shifted the resonant frequency upward

The patch length was adjusted until the resonance aligned with 2.45 GHz.

Final optimized patch length:
- **28.6 mm**

---

## Inset Feed Length Optimization

With the patch length fixed, a parametric sweep was performed on the inset feed
length to improve impedance matching.

Observations:
- Resonant frequency remained approximately constant
- S11 depth changed significantly with inset position

The inset feed length was selected to achieve the minimum S11 near 2.45 GHz.

Final optimized inset feed length:
- **6.0 mm**

---

## Key Takeaways

- Patch length primarily controls resonant frequency
- Inset feed length primarily controls impedance matching
- Separating frequency tuning from matching avoids incorrect optimization

This optimization approach resulted in stable antenna performance within the
2.4 GHz ISM band.
