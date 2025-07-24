# Boost Converter ⚡🔋

## Overview  
This project presents the design, implementation, and analysis of a **Boost Converter** – a DC-DC converter that steps up an input voltage to a higher output. Widely used in **power supplies, electric vehicles**, and **renewable energy systems**, this converter was tested in both **CCM (Continuous Conduction Mode)** and **DCM (Discontinuous Conduction Mode)** using PCB-based implementation and waveform observation.

---

## 🔑 Key Features

### ⚙️ Functionality  
- Boosts DC voltage (input < output)
- Demonstrates both CCM and DCM behavior
- Uses MOSFET-based switching controlled via gate driver
- Analyzes real-world non-idealities

### 🔩 Hardware Design  
- Custom-designed **Gate Driver Circuit**
- Fabricated **Boost Converter PCB**
- Manual soldering and component placement

### 🖥️ Simulation & Measurement  
- PWM signal generation and testing via gate driver
- Oscilloscope used to capture:
  - Inductor current waveform
  - Switch voltage waveform
- Operation validated under various load conditions

### 📉 Theoretical & Practical Comparison  
- Target Output: 20 V  
- Observed Output: 18 V  
- **Efficiency:** ~90%  
- **Error:** 1.36%  
- Included effects of:
  - MOSFET on-resistance
  - Diode forward voltage drop
  - Conduction losses

---

## 🧱 Project Structure

```
boost-converter/
│
├── gate-driver/           # Gate driver design & output testing
│ ├── pcb-layout.png
│ └── pwm-waveform.png
│
├── boost-pcb/             # Boost converter circuit
│ ├── schematic.png
│ ├── layout.png
│ └── fabricated-board.jpg
│
├── waveforms/             # Oscilloscope measurements
│ ├── ccm-inductor-current.png
│ ├── ccm-switch-voltage.png
│ ├── dcm-inductor-current.png
│ └── dcm-switch-voltage.png
│
└── report/ # Final documentation
└── calculations.pdf
```


---

## 👥 Contributors

- **Vansh Raj Singh** – Roll No: 230002079  
- **Nadimpalli Pranav Varma** – Roll No: 230002045  
- **Sidhant Kumar Mohanty** – Roll No: 230002069  
- **Prashant Narang** – Roll No: 230002056  

🧪 **EE252 EMPEL Project | Set E2 Batch B2**

---

## 🙏 Acknowledgments

- **IIT Indore EE Lab** – Equipment & support  
- **Oscilloscope** – For waveform observation  
- **Datasheets & reference designs** – For component selection  
- **Team collaboration** – For circuit soldering and testing

---

## 📝 Observations & Notes

> 📌 *DCM was observed clearly by increasing load resistance.  
> Oscilloscope showed exponential rise/fall of current due to the time constant.*  
>  
> 📉 *Major voltage drop was due to diode forward drop (1.2 V).  
> Switching waveform confirmed efficient energy transfer in CCM.*  
>  
> ✅ *Practical efficiency ~90%, showing strong alignment with theoretical expectations.*

---

