<img width="538" height="137" alt="Screenshot 2025-08-01 161045" src="https://github.com/user-attachments/assets/f3a667c9-07a4-4cc0-b75f-44b1c574a6f3" />

# Zero Birefringence Rib Waveguide

This repository contains a detailed numerical study and simulation of a single-mode silicon-on-insulator (SOI) rib waveguide designed to achieve **zero birefringence**.

## Objective

To design a polarization-independent SOI rib waveguide that:
- Supports single-mode operation for both TE and TM modes.
- Has minimal birefringence, i.e., Δn_eff ≈ 0.

---

## Design Parameters

- Wavelength: 1550–1600 nm
- Core (Si) index: ~3.45
- Cladding (SiO₂) index: ~1.45
- Total height (H): 260–420 nm
- Slab height (h): fixed at 170 nm
- Waveguide width (W): variable

Simulations were conducted using the [EIMS Mode Solver](https://www.computational-photonics.eu/eims.html).

---

## Key Results

| λ (nm) | Width (nm) | H (nm) | h (nm) | Δn_eff | Single Mode |
|--------|-------------|--------|--------|---------|--------------|
| 1590   | 220         | 420    | 170    | 0.00091 | ✅ |
| 1600   | 210         | 420    | 170    | 0.0016  | ✅ |
| 1550   | 300         | 370    | 170    | 0.1758  | ✅ |

> ✅ **Minimum birefringence** of ~0.0009 achieved at λ = 1590 nm with W = 220 nm

---

## File Structure

- `Report.pdf`: Full technical report with simulation results, figures, and analysis
- `figures/`: Cross-section, mode profiles, and Δn_eff vs. W plots (optional if images added)
- `README.md`: Project summary and usage
