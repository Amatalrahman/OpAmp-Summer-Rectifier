# 🎛️ Weighted Summer Circuit – EICN2241

This project demonstrates the design, simulation, and hardware implementation of a **weighted summing amplifier** using an op-amp (TL084/LM324). It's part of the Analog Circuits Lab course – Summer 2024.

---

## 🧠 Overview

We built a simple op-amp circuit that sums two input voltages with equal weights:

Vout = - (V1 + V2)


- **Resistors used**: R₁ = R₂ = R₃ = 100kΩ  
- **Power Supply**: ±12V  
- **Simulation Tool**: MATLAB Simulink  
- **Op-Amps**: TL084 or LM324  

---

## ⚙️ Files Included


📁 weighted-summer-circuit/
├── summer_simulation.slx # Simulink model
├── circuit_schematic.png 


---

## 🔬 What We Did

- Simulated the circuit using Simulink  
- Verified theoretical and simulation outputs match  
- Built the circuit on a breadboard  
- Collected and analyzed practical results

---

## 📈 Results Snapshot

| V₁ (V) | V₂ (V) | V₀ (Expected) | V₀ (Measured) |
|--------|--------|----------------|----------------|
| 2.5    | 3.5    | -6.0           | -5.98          |
| -1.2   | 0.7    | 0.5            | 0.51           |
| 4.8    | -3.2   | -1.6           | -1.61          |

---

## Notes

- Assumes ideal op-amp behavior (virtual ground, infinite gain)  
- Used `ode15s` solver in Simulink  
- Real-world noise and tolerance caused small deviations

## Team 2
- Ziad Mohamed Hamed  
- Amat Al-Rahman Sayed Mohamed  
- Mostafa Hany Tawfik  
- Alaa Essam Abd Alazim  
- Mariam Hosny Abdel-Moneim  
