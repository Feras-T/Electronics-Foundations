# Line Regulator Using a Zener Diode

## Description
This experiment demonstrates the capability of a Zener diode to regulate voltage.  
The Zener diode used has a reverse breakdown voltage of **3.3V**, which ideally remains constant even when the input voltage varies.

A load is connected in parallel with the Zener diode.  
The objective is to observe whether the output voltage across the load changes when the input supply voltage is increased or decreased.

The schematic of the circuit is shown below.

---

## Circuit Diagram
![Schematic](images/Schimatic.png)  
![Real Circuit](images/real_sch.jpeg)

---

## The Experiment

### **Higher Input Voltage**
In this part, the Zener diode is subjected to increasing input voltage to evaluate its ability to maintain regulation.

#### **Input: 15V**
![setting_value_15V](images/setting_value_15V.png)

- Input voltage: **15V**  
- Output voltage across Zener + load: **3.31V**

The Zener holds very close to its rated voltage with minimal deviation.

---

#### **Input: 16V**
![source_value_16V_Output3.35V](images/source_value_16V_Output3.35V.png)

- Input increased by **1V** (from 15V → 16V)  
- Output increases only **~0.04V** (to **3.35V**)

This shows good voltage regulation.

---

#### **Input: 25V**
![power_source_25V_output_3.62V](images/power_source_25V_output_3.62V.png)

- Input increased by **10V** (15V → 25V)  
- Output changes by only **~0.3V** (to **3.62V**)

Even with a large input change, the Zener output remains relatively stable.

---

### **Lower Input Voltage**
![source_value_10V_output_3.31V](images/source_value_10V_output_3.31V.png)

For the lower voltage test, the input is reduced from **15V to 10V**.

- Input drop: **5V**  
- Output drop: only **~0.3V** (from 3.3V → ~3.1V)

This indicates that the Zener diode maintains regulation reasonably well even when the input voltage decreases, as long as the diode remains in its breakdown region.

---

## Conclusion
The Zener diode is capable of acting as a simple voltage regulator.  
From the experiment, we observe:

- The Zener diode regulates **better at higher input voltages** (strong breakdown region).  
- Output voltage changes very little compared to large variations in input voltage.  
- Regulation becomes weaker when the input voltage drops close to the Zener breakdown threshold.

Overall, the Zener diode provides effective voltage regulation for low-current, low-precision applications.

