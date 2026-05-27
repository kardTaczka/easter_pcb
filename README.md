# Easter PCB

## Quick view of PCB

Below are presented screenshots of 3d render PCB and schematic.

### 1. Front
![Front](photos/front.png)

### 2. Back
![Back](photos/back.png)

### 3. Schematic
![Schematic](photos/schematic.png)

---

## About
**Dual-Channel Alternating Output** -  The NE555 timer operates at approximately 0.2 Hz. Its square wave output is smoothed by an RC integration network consisting of a 10 kΩ resistor and a 50 µF capacitor bank (achieved by placing five 10 µF MLCCs in parallel). This analog signal drives a complementary transistor pair consisting of a BCP56 (NPN) and a BCP53 (PNP). 

Instead of driving a single array, the load is split into two separate LED rails. Because the NPN and PNP transistors conduct on opposite voltage swings, they create an alternating "breathing" effect. When the capacitor charges, the NPN rail fades in while the PNP rail fades out. When the voltage drops, the cycle reverses. The peak forward current is hardware-limited to a safe and visually pleasing 3 mA per LED.
