#  Weighted Summer & Rectifier Circuit 


## Overview

This project combines two essential analog electronics concepts in a single circuit:
- **Weighted Summing Amplifier** using an op-amp (TL084/LM324)
- **Full-Wave Bridge Rectifier** with capacitor filtering

The circuit was built, simulated using **MATLAB/Simulink**, and tested practically. The results were compared across theoretical, simulated, and measured domains.

---

## Objectives

- Implement a summing amplifier circuit with equal weights.
- Simulate a full-wave rectifier with smoothing.
- Compare expected and actual output voltages.
- Observe ripple before and after filtering.

---

## ⚙️ Circuit Description

### Summing Amplifier

- Op-amp configuration with equal resistors:  
  \[
  R_1 = R_2 = R_3 = 100\,k\Omega
  \]
- Output voltage:  
  \[
  V_0 = - (V_1 + V_2)
  \]
- Assumes ideal op-amp:  
  - Infinite gain (A → ∞)  
  - Virtual short: \(V^- \approx V^+\)  
  - Virtual ground at \(V^- \approx 0\)  

### Bridge Rectifier

- 4 × 1N4007 diodes in a full-wave bridge.
- Smoothing capacitor (e.g., 1000 µF).
- Load resistor: 1 kΩ.
- Output observed before and after filtering.

---

## Simulation & Testing

### Tools Used
- **Simulink** (MATLAB)
- **Digital Multimeter**
- **Oscilloscope** (optional)

### ⚡ Inputs & Outputs

| AC Input (V) | Expected DC (V) | Measured DC (V) | Error (mV) |
|--------------|------------------|------------------|------------|
| 10           | 9.3              | 9.25             | 50         |
| 6            | 5.3              | 5.21             | 90         |
| 2            | 1.3              | 1.17             | 130        |

- **Ripple** reduced significantly after filtering.
- **Voltage drop** due to diode (~0.7V) taken into account.

---

## 📈 Observations

- Simulation models ideal components → results slightly higher than measured.
- Adding a capacitor significantly reduced ripple.
- Output voltage remained stable under different loads.

---

## Conclusion

The project successfully demonstrated:
- Summing two signals using an op-amp.
- Converting AC to DC using a full-wave rectifier.
- The importance of filtering and component behavior.

Applications:
- Analog computation  
- Power supplies & DC converters  
- Signal conditioning in embedded systems

---

## 📁 Project Files





---

## Team 
- Ziad Mohamed Hamed  
- Amat Al-Rahman Sayed Mohamed  
- Mostafa Hany Tawfik  
- Alaa Essam Abd Alazim  
- Mariam Hosny Abdel-Moneim  


