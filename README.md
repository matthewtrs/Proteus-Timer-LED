# PulseSync (Motion Sensor Light)

**Team Members**:  
Hezekyah Gokbasa, Jefferson Siagian, Matthew Tristan Hutapea, Jevon Nobel Napitupulu, Daffa Farrell Dewanto

---

## Problem

In today's globalized world, almost all human activities require electrical energy. From household activities, offices, shops, factories, to personal activities, electricity is essential. Without it, these activities would be disrupted or even impossible.

Electricity is not an easily obtained energy source, as it depends on natural resources that are not infinite. Excessive use of electricity leads to negative impacts such as global warming, increased greenhouse gas emissions, rolling blackouts, reduced future energy reserves, extreme weather, and inflated electricity bills.

As users of electrical energy, we must be aware of the importance of saving electricity to protect our planet. However, many people still lack this awareness, even though saving electricity is easy. Simple actions like turning off lights or electronic devices when not in use can make a difference. Surveys show that electricity waste is often related to habits, such as leaving lights on continuously.

PulseSync aims to help reduce electricity waste by automatically turning off lights when they are not in use.

---

## Ideas

Our project, PulseSync, is a motion sensor device designed to save electricity by controlling lighting. The system is applied in rooms where human activities occur. It detects heat and automatically turns on the lights when someone enters the room or stands under the light. When the person leaves, the lights turn off after a few seconds. A manual button is also provided for users to turn the lights on or off manually. If the user forgets to turn off the lights, they will automatically turn off after the person leaves the room.

---

## Theory & Implementation

The system uses an IR sensor and implements an XNOR lock system for countdown control. The XNOR gate outputs a high signal when both inputs are the same. In this system, a 4-bit BCD code from the Set Counter and Running Counter is compared. If the values match, the light turns off.

### Modules:

1. **Module 1 (Circuit Introduction)**  
   Introduces the core concepts of the PulseSync circuit.

2. **Module 2 (Boolean Algebra)**  
   Applies Boolean algebra to create logic gate combinations (AND, OR, NOT) for the circuit.

3. **Module 3 (Karnaugh Map)**  
   Optimizes and simplifies logic gate design.

4. **Module 4 (Complex Logic Gates)**  
   Uses XNOR gates for the 4-bit lock system, comparing Set Counter and Running Counter values.

5. **Module 5 (Encoder and Decoder)**  
   Uses IC 7448 to convert 4-bit BCD codes to 7-segment display outputs.

6. **Module 6 (Mux and Demux)**  
   Uses IC 4555 as a 1:2 demultiplexer to control light changes.

7. **Module 7 (Arithmetic Digital Circuit)**  
   Implements a ripple carry adder (IC 74LS83) for 7-segment display optimization.

8. **Module 9 (Register and Counter)**  
   Uses IC 74192 as a counter to control light timing.

---

## Result & Analysis

The PulseSync circuit was successfully simulated and produced the expected output. The system controls light activation and deactivation based on the presence or absence of individuals detected by the IR sensor. When the sensor detects someone, the light turns on, and when the person leaves, the light turns off after a set time (0-9 seconds) using the 4-bit XNOR lock system.

Two 7-segment displays are used: one for setting the counter (Set Counter) and one for the running count (Running Counter). The light turns off when the 4-bit BCD values of the Set Counter and Running Counter match.

---

## Conclusion

PulseSync aims to save electrical energy by using motion sensors and light control systems. The IR sensor detects human presence, automatically turning the light on when someone is in the room and off when they leave. The project is based on the importance of saving electricity to protect the environment and reduce negative impacts like global warming and greenhouse gas emissions.

The circuit uses XNOR gates for the 4-bit lock system, comparing Set Counter and Running Counter values. Other components like encoders, decoders, and demultiplexers are also used. PulseSync contributes to energy conservation by automatically turning off lights when not in use.

---

## References

1. GeeksforGeeks, “BCD to 7 segment decoder,” [Online]. Available: [https://www.geeksforgeeks.org/bcd-to-7-segment-decoder/](https://www.geeksforgeeks.org/bcd-to-7-segment-decoder/)
2. ElectronicsHub, “What is Demultiplexer,” [Online]. Available: [https://www.electronicshub.org/demultiplexer-demu x/](https://www.electronicshub.org/demultiplexer-demu x/)
3. ICRFQ, “Counter IC,” [Online]. Available: [https://www.icrfq.net/counter-ic/](https://www.icrfq.net/counter-ic/)
4. Electronics For You, “555 Timer - Working, Specifications, and Applications,” [Online]. Available: [https://www.electronicsforu.com/technology-trends/learn-electronics/555-timer-working-specification](https://www.electronicsforu.com/technology-trends/learn-electronics/555-timer-working-specification)
5. Fierce Electronics, “What Is an IR Sensor?,” [Online]. Available: [https://www.fierceelectronics.com/sensors/what-ir-sensor](https://www.fierceelectronics.com/sensors/what-ir-sensor)
6. Easy Electronics Project, "Motion Sensor Light with IR Proximity Sensor and 4017," [Online]. Available: [https://easyelectronicsproject.com/mini-projects/motion-sensor-light-ir-proximity-sensor-4017/](https://easyelectronicsproject.com/mini-projects/motion-sensor-light-ir-proximity-sensor-4017/)
7. Guru Elektronika, “Cara Kerja Sensor Infra Red - Beserta Cara Membuat Rangkaiannya,” [Online]. Available: [https://www.youtube.com/watch?v=kv9sB8fAM](https://www.youtube.com/watch?v=kv9sB8fAM)

---

## Circuit Diagram

![Circuit Diagram](circuit_diagram.png)
