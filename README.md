# Laboratory Mice Automatic Feeder
Automated and autonomous laboratory mice feeder powered by ESP8266, covered with a  brass shield (anti-gnawing).
This repository features an automated and fully autonomous rodent feeder designed for laboratory environments. It allows precise control over feeding schedules through a motorized rotating drum mechanism.
The device is completely battery-powered to avoid human intervention during feeding time.

---
## Operating Principle
The system operates using a physical rotary barrier mechanism:
* **Structure:** A main external cylinder features an access "window". Inside, a rotating drum, containing food, is split into two halves: one solid wall and one open side fitted with stainless steel bars.
* **Locked Mode (Rest):** The solid wall of the drum aligns with the external window, completely blocking access to the food.
* **Feeding Mode:** At scheduled times, a servo motor rotates the drum on its vertical axis to align the stainless steel bars side with the window, allowing the mice to feed.

---
## Technical Specifications and Bill of Materials

### 3D Printed Parts (PLA)
All source and print files are available in the 'hardware/mechanical/' directory.
* 'cylindre_exterieur.stl': Main housing structure featuring the feeding window.
* 'tambour.stl' and 'anneau_tambour.stl': Internal drum holding the food and steel bars and the ring that holds the bars in place into the drum.
* 'bouchon_haut.stl' and 'bouchon_bas.stl': Enclosures for the main cylinder, with cavities to place O-rings.
* 'pièce_partie_electronique.stl': Internal fixture for components located beneath the drum.

 ### Protection Materials and Fasteners
 * **Brass sheets:** Applied to the external cylinder and the outer wall of the drum to prevent the mice from chewing through the PLA plastic.
 * **Stainless steel bars:** Fitted onto the feeding side of the drum and the holding ring.

### Electronics and Power
Circuit diagrams can be found in the 'hardware/schematics/' directory.
* **Microcontroller:** ESP8266.
* **Actuator:** Servo motor SG90 (coupled to the vertical axis of the drum).
* **Clock:** RTC DS1307.
* **Power Supply:** 2x 3.7V Li-ion batteries.
* **Step-Down Converter:** to convert the >7V of both batteries into 5V for the Servo Motor.
* Various wiring and connectors.

---
## Repository Structure
* '/firmware': Arduino source code ('.ino') for the ESP8266, RTC, and servo management.
* '/harware/mechanical': 3D models in '.STL' format.
* '/hardware/schematics': Electronics wiring and and other schematics.
* '/docs': Additional documentation and assembly/use guides

---
## The Team 
This project was co-developed with pride by:
* **ZEMLYANOI Macha** - Firmware and Electronics
* **SERET Lucas** - Hand-drawn Schematics and Mechanical/Electronical Conception
* **MMADI Zainaba** - 3D Modeling and Documentation

This project was fully realized at **FabLab UniCA**.

