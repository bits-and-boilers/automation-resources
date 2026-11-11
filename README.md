# Automation Resources

A curated, beginner-to-advanced list of free and low-cost resources for learning **PLC programming, industrial controls, and OT (operational technology)**, written especially for people crossing over from IT.

Maintained by [Kevin Plouffe](https://github.com/bits-and-boilers). Suggestions welcome: open an issue.

**Cost key:** 🆓 free · 💲 free tier or trial, paid for full use · 📕 paid

---

## Level 1: Fundamentals

*How a PLC works, ladder logic basics, and your first programs on a simulator.*

### Learn
- 🆓 [PLC Practice](https://www.plcpractice.com/): practice problems to build ladder-logic fluency.
- 📕 [PLC Dojo: PLC Fundamentals](https://www.plcdojo.com/courses/plc-fundamentals): a structured fundamentals course.
- 🆓 [PLC Academy](https://www.plcacademy.com/): free tutorials on how PLCs work and how to program them.
- 🆓 [SolisPLC Tutorials](https://www.solisplc.com/tutorials): free articles and videos on ladder logic, Allen-Bradley, and Siemens.
- 🆓 [AutomationDirect Free Video Tutorials](https://cdn.automationdirect.com/static/press/video_tutorials_plc.html): "What is a PLC?" series plus hands-on CLICK and Do-more walkthroughs.
- 💲 [RealPars: How to Learn PLC Programming](https://www.realpars.com/blog/how-to-learn-plc-programming): a good roadmap article. RealPars' YouTube channel is free; full courses are a subscription.

### Practice (no hardware needed)
- 🆓 [AutomationDirect Do-more Designer](https://www.automationdirect.com/do-more/brx/software): free, fully functional programming software with a built-in PLC simulator. Probably the easiest real-world vendor tool to start on.
- 🆓 [OpenPLC](https://autonomylogic.com/): open-source, IEC 61131-3 compliant PLC. Run it as a soft PLC on your PC or on a Raspberry Pi or Arduino.

---

## Level 2: Building Real Logic

*All five IEC 61131-3 languages, structured text, timers, counters, sequences, and state machines, plus simulated machines to control.*

### Tools
- 🆓 [CODESYS Development System](https://us.store.codesys.com/codesys.html): free, industry-standard IEC 61131-3 IDE with a soft PLC for testing. The same environment sits underneath many commercial PLC brands.
- 💲 [Factory I/O](https://factoryio.com/): 3D factory simulator (conveyors, sorters, sensors) you control from a real or simulated PLC. 30-day free trial, then paid.

### Learn
- 🆓 [PLCopen](https://www.plcopen.org/): the user organization behind IEC 61131-3. Background on the standard and good programming practice.

### Project ideas
Classic exercises worth building and posting:
- Traffic light with pedestrian request
- Start/stop motor circuit with seal-in and fault latch
- Conveyor with photo-eye counting and a full-bin stop
- Tank fill/drain with high/low level alarms
- Sorting line in Factory I/O

---

## Level 3: Systems, Networks, and OT

*How PLCs talk to each other, to HMIs and SCADA, and to the business; and how to keep it all secure.*

### Industrial networks
- 🆓 [Modbus Organization FAQ](https://www.modbus.org/faq): what Modbus is, where it came from, and where to get the free specification. It's the simplest industrial protocol to learn first.
- 🆓 [pymodbus](https://github.com/pymodbus-dev/pymodbus): Python library for Modbus TCP/RTU. A great bridge if you already script.
- 🆓 [Node-RED](https://nodered.org/): low-code flow tool widely used for quick HMI dashboards and protocol bridging.

### HMI / SCADA
- 🆓 [Inductive University](https://inductiveuniversity.com/): free, self-paced training and credentials for Ignition SCADA, with a free trial of the software to practice on.

### Standards (good to know by name)
- 📕 [ISA-95](https://www.isa.org/standards-and-publications/isa-standards/isa-95-standard): how plant-floor control systems integrate with business systems (MES, ERP). This is the IT-to-OT boundary.
- 📕 [ISA/IEC 62443](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards): the main cybersecurity standard series for industrial automation and control systems.

### OT security
- 🆓 [CISA ICS Training](https://www.cisa.gov/ics-training-available-through-cisa): free on-demand and instructor-led industrial control system cybersecurity courses from the U.S. government.

---

## Coming from IT

If you're coming from enterprise IT, a lot transfers. Some things work very differently, though.

**What carries over**
- **Networking:** VLANs, subnets, firewalls, and troubleshooting connectivity are daily work in modern plants.
- **Change control and documentation:** runbooks, version control, and rollback plans matter even more when a bad change stops a production line.
- **Systems thinking:** integrating platforms, managing vendors, and owning uptime.
- **Scripting:** Python and SQL show up in data collection, historians, MES, and testing.

**What's different**
- **Safety comes first, then availability, then confidentiality.** The priority order is roughly the reverse of IT.
- **Equipment lives 15–30 years.** You can't just patch or reboot a controller that's running a line.
- **Determinism.** PLCs run a fixed scan cycle, and timing is part of correctness.
- **The floor is the customer.** Operators, maintenance techs, and electricians are the people you serve. Spend time with them.

### Community
- 🆓 [r/PLC](https://www.reddit.com/r/PLC/): active community of controls engineers; good for questions and career advice.

---

## Contributing

Know a great free resource? Open an issue or pull request with the link, the level it belongs in, and one line on why it's worth someone's time.
