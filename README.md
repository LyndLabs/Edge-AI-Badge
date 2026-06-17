# Edge AI Foundation Badge

![](/assets/v0-edge-ai-badge.jpg)  

The Edge AI Badge lets you plug-and-play with the latest vendor hardware at conference workshops and wirelessly connect with other attendees! Use the badge to explore the Edge AI curriculum, plug into sensors, and start building apps.

- 📄 [Read the docs →](https://lyndlabs.github.io/edge-ai-badge-docs)
- 💻 [Download or contribute to firmware](https://github.com/lyndlabs/edge-ai-badge-firmware).

## Hardware 
The badge is a modular PCB that allows you to customize your own face & backplates - the hardware platform is consistent at future conferences and makes it easy for attendees to design their own add-ons, or vendors that want to contribute hardware. 

It's built around the ESP32-S3, selected for its cryptographic core + secure boot, communication protocols (WiFi, BLE, ESP-NOW), infrared hardware, native USB, and ubiquitous support.

---

## Contents
- **assets**: logos, renders, global design assets
    - *find local assets under subfolders*
- **pcb**: KiCAD design files for `main`, `face`, `back`
- **fab**: production-ready pcb + laser files

## Versions & Notes
Versions bumped per batch release, revisions tracked for minor design changes per board - `main`, `face`, `back` tracked separately.

### v1 
- [x] Fixed USB + Power Path + XTAL issue 
- [ ] Buttons on resistor ladder
- [ ] Power button to MCU
- [ ] Standoff drill
- [ ] Interrupt to expansion
- [ ] Diode on USB 

### v0 - 26/06/08
- Main boards + backplate only - released in green HASL
- Wrong SMD standoff drilling size + CPL in production batch - used regular standoffs
- CPL + BOM discrepancy, released for visibility but pls do not order
- Known issue with USB charging
- Known issue w. Deep Sleep (.1uF caps on xtal)
