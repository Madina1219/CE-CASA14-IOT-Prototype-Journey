# Prototyping the Internet of Things – Connected Environments Journey  
*A reflective exploration of IoT design, prototyping, and environmental insight through the CASA0014 module at UCL.*

---

## About the Module
**Prototyping the Internet of Things (CASA0014)** explores how digital connectivity and sensing technologies shape our built environment.  
This repository documents my full journey through the module, combining lecture insights, practical experimentation, prototyping, and reflective learning.

The course covered:
- **L1:** Introduction to IoT and its role in the built environment  
- **L2:** Sensors, actuators, and how devices communicate  
- **L3:** Gateways, data exchange protocols, and MQTT communication  
- **L4:** Field exploration of real IoT systems at the Queen Elizabeth Olympic Park  
- **L5:** Arduino and microcontrollers as the "brains" of IoT systems  
- **L6:** One-minute prototype pitch and concept development  
- **L7:** Prototyping as a process of learning, iteration, and creative thinking  

---

## 🔍 Learning Reflections

### **Understanding IoT in Context**
I learned how the Internet of Things connects data, people, and infrastructure to create responsive and intelligent environments.  
Through examples shared in lectures, I reflected on how IoT can address sustainability, mobility, and energy challenges in urban life.

### **Sensors and Actuators**
Hands-on exploration of sensors and actuators helped me understand how data is captured and acted upon. I experimented with environmental and sound sensors, learning how signal noise, calibration, and environment affect reliability.

### **Gateways and Protocols**
Working with **MQTT** introduced me to lightweight messaging between devices and servers. I understood how topic-based communication enables scalable IoT networks and the importance of consistent naming conventions and security.

### **Field Study – QEOP Walk**
Seeing real-world IoT installations across the **Queen Elizabeth Olympic Park** (environmental sensors) showed me how technology and design intersect in public spaces.  
It deepened my awareness of privacy, maintenance, and long-term value in connected urban systems.

### **Arduino and Microcontrollers**
Building with the **MKR WiFi 1010** taught me to think like both an engineer and a designer, understanding how hardware, software, and user interaction intertwine.  
I learned coding structures, debugging, WiFi connectivity, and MQTT publishing through trial and error.

### **Prototyping and Iteration**
I discovered that prototyping isn’t only about achieving a perfect product, but also about thinking through making, testing ideas physically to understand limitations, user experience, and potential improvements.

---

## Prototype: “Chrono Lumina”  

**Concept:**  
A sound-activated IoT lighting system that responds to a rhythmic “3-knock” trigger, controlling a **Vespera** light installation via MQTT.  

**Core Features:**
- Arduino MKR WiFi 1010 microcontroller  
- MAX4466 analog microphone sensor  
- MQTT communication through `mqtt.cetools.org`  
- Real-time LED control sequence (Blue → Red → Green)  
- Exact 3-knock detection logic with adaptive timing  

**Challenges:**  
During live demonstration, unexpected environmental noise and acoustic interference caused false triggers. The prototype revealed how changes in environment, microphone gain, and human rhythm influence IoT performance.

**Lessons Learned:**  
Knock detection is less about loudness and more about robust signal processing. I learned the value of adaptive thresholds, environmental calibration, and mechanical isolation in IoT reliability.

**Next Steps:**  
- Implement adaptive thresholding (baseline + k·σ)  
- Integrate transient shape analysis and calibration steps  
- Improve user feedback (LED indicators)  
- Test alternative inputs such as piezo or accelerometer sensors  
