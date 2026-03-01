# Antenna Performance Summary

This document summarizes the final simulated performance of the
2.45 GHz microstrip patch antenna after optimization.

All results were obtained using CST Studio Suite.

---

## Impedance Matching

| Metric | Value |
|------|------|
| Resonant frequency | ~2.46 GHz |
| Minimum S11 | ~−22.8 dB |
| VSWR @ 2.45 GHz | ~1.24 |

The antenna exhibits good impedance matching within the 2.4 GHz ISM band.

---

## Radiation Characteristics

| Parameter | Value |
|---------|------|
| Radiation type | Broadside |
| Main lobe direction | Normal to patch (+Z) |
| Polarization | Linear |

The radiation pattern shows a single dominant main lobe with stable behavior
at the operating frequency.

---

## Gain and Efficiency

| Parameter | Value |
|---------|------|
| Peak realized gain | ~1.73 dBi |
| Radiation efficiency | ~41% |
| Total efficiency | ~40% |

The relatively low realized gain is expected due to the lossy FR4 substrate
and compact ground plane dimensions.

---

## Validation

- E-field is concentrated at the patch edges, confirming fringing-field radiation.
- H-field is concentrated beneath the patch and near the feed, indicating correct
  surface current distribution.

---

## Remarks

The antenna performance is suitable for compact 2.4 GHz ISM-band applications
where low cost and small size are prioritized over high gain.
