# Source Degenerated CS Amplifier Variations

**Tool:** LTSpice  
**Technology:** 180 nm CMOS  
**VDD:** 1.8 V  
**Load Capacitance:** 1 pF  

---

# Aim

To design and compare three source-degenerated Common-Source (CS) amplifiers in terms of:

- DC bias  
- Gain  
- Linearity  
- Bandwidth  
- Power consumption  

---

# 1️⃣ Resistive Source Degeneration (Rs)

## Key Components

| Component | Value |
|------------|--------|
| NMOS (M1) | W = 390 nm, L = 180 nm |
| PMOS (M2) | W = 1.5 µm, L = 180 nm |
| Rs | 15 kΩ |
| VDD | 1.8 V |
| CL | 1 pF |

---

## DC Results

- **ID ≈ 3.5 µA**
- **Vout ≈ 0.9 V**
- **Power ≈ 6.3 µW**

Satisfies power constraint (< 20 µW).

---

## AC Performance

- **Gain:** 18–20 dB  
- **Linear Gain:** 8–10  
- **Bandwidth:** Moderate  

---

## Observation

- Rs introduces local negative feedback.  
- Gain reduces compared to basic CS.  
- Linearity improves.

---

# 2️⃣ MOS Source Degeneration (Fixed VBN)

## Key Components

| Component | Value |
|------------|--------|
| M1 | W = 390 nm |
| M2 | W = 1.5 µm |
| M3 | W = 180 nm |
| L (All) | 180 nm |
| VBN | 0.55 V |

M3 operates in linear region and behaves as a voltage-controlled resistor.

---

## DC Results

- **ID ≈ 3.8 µA**
- **Vout ≈ 0.9–1.0 V**
- **Power ≈ 6.8 µW**

Within limit.

---

## AC Performance

- **Gain:** 14–16 dB  
- **Linear Gain:** 5–6  
- **Bandwidth:** Higher than Rs case  

---

## Observation

- Gain decreases further.  
- Bandwidth increases.  
- Fully CMOS compatible.  
- Resistance depends on bias voltage.

---

# 3️⃣ Gate-Tied MOS Degeneration (Self-Biased)

- Gate of M3 tied to input.
- No external bias (VBN).
- Strongest feedback among three.

---

## DC Results

- **ID ≈ 3–4 µA**
- **Vout ≈ 0.87–0.9 V**
- **Power ≈ 6–7 µW**

Meets power requirement.

---

## AC Performance

- **Gain:** 10–12 dB  
- **Linear Gain:** 3–4  
- **Bandwidth:** Highest  

---

## Observation

- Lowest gain.  
- Best linearity.  
- Strong local feedback improves stability.

---

# Comparison Summary

| Parameter | Rs | MOS (Fixed) | Gate-Tied |
|------------|------|-------------|-----------|
| ID | ~3.5 µA | ~3.8 µA | ~3–4 µA |
| Power | ~6.3 µW | ~6.8 µW | ~6–7 µW |
| Gain (dB) | 18–20 | 14–16 | 10–12 |
| Linear Gain | 8–10 | 5–6 | 3–4 |
| Bandwidth | Moderate | Higher | Highest |
| Linearity | Good | Better | Best |
| CMOS Friendly | No | Yes | Yes |

---

# Overall Findings

- Source degeneration lowers gain.
- Linearity improves due to negative feedback.
- MOS-based degeneration enhances integration.
- Gate-tied configuration provides strongest feedback and widest bandwidth.
- Gain–bandwidth tradeoff clearly observed.
- All designs consume less than 20 µW.

---

# Conclusion

Three source-degenerated CS amplifiers were implemented and compared in 180 nm CMOS.  

The results confirm:

- Effectiveness of source degeneration  
- Tradeoff between gain and bandwidth  
- Feedback-driven linearity improvement  
- Advantages of MOS-based implementation in IC design  
