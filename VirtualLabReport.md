# THE NATIONAL INSTITUTE OF ENGINEERING  
**Mysuru – 570 008**

# VIRTUAL LAB REPORT  

## COURSE DETAILS

**Course:** Linear Integrated Circuits  
**Course Code:** BEC405D  

---

## Submitted By

**Name:** Ashish R Mestha  
**USN:** 4NI24EC021  
**Semester:** IV  
**Section:** A  

---

## Submitted To

**Dr. Yajunath K**  
Assistant Professor  
Department of ECE  
The National Institute of Engineering  
Mysuru  

---

## Academic Year: 2025–2026  

---

# Experiment

## Measurement of Input Bias Current, Input Offset Current, Input Offset Voltage, Output Offset Voltage and Slew Rate of IC 741

---

# Aim

To experimentally determine the non-ideal parameters of the IC 741 operational amplifier using a virtual laboratory setup. The parameters measured include:

- Input Bias Current  
- Input Offset Current  
- Input Offset Voltage  
- Output Offset Voltage  
- Slew Rate  

---

# Apparatus Required

- IC 741 Operational Amplifier  
- Dual DC Power Supply (+Vcc and −Vcc)  
- Digital Multimeter  
- Function Generator  
- Connecting Wires  

---

# Theory

An ideal operational amplifier is assumed to have infinite input impedance, zero input current, zero offset voltage, and infinite bandwidth. However, practical op-amps such as the **IC 741** exhibit small deviations from these ideal characteristics.

### 1. Input Bias Current (IB)

Input bias current is the average of the currents entering the inverting and non-inverting terminals.

\[
IB = \frac{IB1 + IB2}{2}
\]

Where:  
IB1 = Inverting input current  
IB2 = Non-inverting input current  

---

### 2. Input Offset Current (IOS)

Input offset current is the difference between the two input bias currents.

\[
IOS = |IB1 - IB2|
\]

It indicates the mismatch between the input transistors of the op-amp.

---

### 3. Input Offset Voltage (VIO)

Input offset voltage is the small differential input voltage that must be applied between the input terminals to make the output voltage zero.

---

### 4. Output Offset Voltage

It is the output voltage observed when the input terminals are grounded. Ideally, this should be zero, but due to internal transistor mismatches, a small output voltage exists.

---

### 5. Slew Rate (SR)

Slew rate is the maximum rate at which the output voltage changes with respect to time.

\[
SR = \left( \frac{dV_o}{dt} \right)_{max}
\]

Unit: V/µs  

It determines how fast the op-amp can respond to rapid changes in input.

---

# Circuit Measurements

The following parameters were obtained through simulation and measurement in the virtual lab environment.

---

# Observation Table

| Sl. No | Parameter | Measured Value |
|---------|-----------|----------------|
| 1 | Input Bias Current | Inverting: 0.051 µA |
|   |  | Non-inverting: −0.0425 µA |
| 2 | Input Offset Current | 0.0063 µA |
| 3 | Input Offset Voltage | 1.049 mV |
| 4 | Slew Rate | 0.471 V/µs |

---

# Result

The important non-ideal characteristics of the IC 741 operational amplifier were measured successfully using the virtual lab setup. The obtained values of input bias current, offset current, offset voltage, and slew rate are within the expected practical range for a 741 op-amp.

---

# Conclusion

This experiment demonstrated that real operational amplifiers do not behave ideally. The IC 741 exhibits measurable input bias current, input offset current, input offset voltage, and a finite slew rate. These parameters affect the performance of amplifier circuits, particularly in precision and high-frequency applications.

The virtual experiment effectively verified the theoretical concepts of op-amp non-idealities and provided practical insight into the limitations of the IC 741.
