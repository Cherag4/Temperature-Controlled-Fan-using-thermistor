# Temperature Controlled Fan Using Op-Amp Comparator

## 📌 Overview
This project demonstrates a temperature-controlled fan circuit using an op-amp configured as a comparator and an NTC thermistor for temperature sensing. The fan automatically turns ON when the temperature exceeds a preset threshold and turns OFF when it falls below it. The circuit is designed and verified using LTspice.

---

## 🎯 Objectives
- Sense ambient temperature using a thermistor  
- Compare temperature with a reference voltage  
- Automatically control a cooling fan  
- Validate operation through LTspice simulation  

---

## 🧩 Components
- Op-Amp (Comparator)
- NTC Thermistor (10kΩ, β = 3950)
- NPN Transistor (2N2222)
- Diode (1N4007)
- Resistors
- 12V DC Supply
- Fan (modeled as load)

---

## ⚙️ Working Principle
- The thermistor and resistor form a voltage divider whose output varies with temperature.
- An op-amp compares this voltage with a fixed reference.
- When the temperature crosses the threshold, the op-amp output goes HIGH.
- A transistor amplifies the current to drive the fan.
- A flyback diode protects the transistor from inductive spikes.

---

## 🧪 Simulation Details
- Software: LTspice  
- Supply Voltage: 12V  
- Temperature Range: 20°C – 80°C  
- Analysis: DC sweep using .step command  

---

## 📊 Results
- Fan OFF below ~38°C  
- Fan ON above threshold temperature  
- Sharp switching confirms correct comparator behavior  

---

## ✅ Features
- Simple analog design  
- No microcontroller required  
- Low cost and reliable  
- Fast response  

---

## 🔧 Future Improvements
- Add hysteresis to avoid rapid switching  
- Implement PWM-based speed control  
- Hardware implementation  

---

## 📚 References
- Sedra & Smith, *Microelectronic Circuits*  
- LTspice Documentation  
- 2N2222 and 1N4007 Datasheets
