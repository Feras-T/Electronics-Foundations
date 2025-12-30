# Vlotage Regulator Using a Zener Diode

## Objective
This experiment demonstrates the ability of a Zener diode to regulate the output voltage by operating in its reverse-breakdown region.
 

## Background Theory
A Zener diode is primarily used to maintain a stable reference voltage by operating in its controlled reverse-breakdown region, making it suitable for simple voltage regulation and over-voltage protection in electronic circuits.

---

## Circuit Diagram
![Schematic](images/Schimatic.png)

The Zener diode is reverse-biased and connected in parallel with the load.
A 1 kΩ resistor is placed in series between the power supply and the Zener–load node to limit the current.
The load consists of a red LED in series with a 330 Ω resistor.


---

## Components & Instruments
| Item | Specification |
|----|-------------|
| Diode | 3.3 Vz |
| Resistor | 1 kΩ ±5% |
| Resistor | 330 Ω ±5% |
| LED | Red LED, Vf ≈ 2.0 V, If ≈ 10–20 mA |
| Multimeter | Digital |
| Power Supply | 0–30 V |

## Experimental Setup
![Real Circuit](images/real_sch.jpeg)


The Zener diode used has a reverse breakdown voltage of **3.3V**, which ideally remains constant even when the input voltage varies.

A load is connected in parallel with the Zener diode.  
The objective is to observe whether the output voltage across the load changes when the input supply voltage is increased or decreased.


## 6. Procedure
1. Set power supply to 15 V.
2. increase the power supply voltage up to 25V.
2. Measure Load voltage while increasing the power supply voltage.
4. Compare load voltage values with power suplly value.


## Measurements
| Power Supply Voltage (V) | Load Voltage (Zener Voltage) |
|------------|-------------|
| 15 | 3.31 V |
| 16 | 3.35 V |
| 25 | 3.62 V |



#### **Input: 15V**
![setting_value_15V](images/setting_value_15V.png)

---

#### **Input: 16V**
![source_value_16V_Output3.35V](images/source_value_16V_Output3.35V.png)
---

#### **Input: 25V**
![power_source_25V_output_3.62V](images/power_source_25V_output_3.62V.png)

## 8. Results & Analysis
The input power supply voltage was increased from 15 V to 25 V (ΔV = 10 V), while the load voltage changed by only 0.31 V.
With a 10 V input and a 1 kΩ series resistor, the Zener diode produced an output of approximately 3.0 V rather than its nominal 3.3 V due to insufficient Zener current for proper regulation.

## Discussion
In practical designs, insufficient Zener current can lead to poor voltage regulation, which limits the suitability of Zener diodes for precision voltage regulation in embedded systems.
 
## 11. Lessons Learned
 -Zener diodes provide a simple and rough method for voltage regulation.
 -The Zener diode performance strongly depends on the operating current, and insufficient Zener current can result in poor regulation.

## Conclusion
This experiment demonstrated the voltage regulation behavior of a Zener diode in a shunt regulator configuration, while also showing that insufficient Zener current leads to reduced regulation accuracy.


---

### **Lower Input Voltage**
![source_value_10V_output_3.31V](images/source_value_10V_output_3.31V.png)

For the lower voltage test, the input is reduced from **15V to 10V**.

- Input drop: **5V**  
- Output drop: only **~0.3V** (from 3.3V → ~3.1V)

This indicates that the Zener diode maintains regulation reasonably well even when the input voltage decreases, as long as the diode remains in its breakdown region.

---
