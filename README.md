Tinashe Chingwaru

Electronic engineer · Cape Town, South Africa

From the PCB to the software that runs it. I design and maintain networked embedded products end to end: the board, the firmware on the microcontroller, the PC and mobile software that talks to it, and the production tests that prove each unit works.

Focus: embedded firmware, hardware design, C#/.NET systems
Sector: access control, intercom and security equipment
Degree: BEng Electrical and Electronic Engineering, University of Johannesburg (2017–2020)
Registration: working towards Pr Eng (ECSA)

Portfolio · LinkedIn · Email

What I work with
Area	Tools and skills
Embedded firmware	C on STM32, FreeRTOS, LwIP, UDP, DeviceNet, Wiegand, Bluetooth Low Energy
Hardware	Altium Designer, schematic and PCB layout, isolated outputs, power conversion, surge and ESD protection
Software	C#/.NET (WinForms, WPF), multithreading, MySQL, Android
Test and QA	Production test design, test jigs, root-cause analysis, defect tracking, release review
Bench	Oscilloscope and multimeter fault-finding, fine-pitch SMD rework
Selected work

These are commercial projects, so the source code is not public, and client, site and product names are left out. I'm happy to talk through the engineering.

Fleet management system for networked safes

C# MySQL UDP Multithreading

Turned a single-user diagnostic tool into a multi-user server/client system, roughly doubling the codebase.

Server/client architecture around a shared MySQL database, with a server heartbeat that clients watch
Thread-safe UDP layer, with database writes moved to a queue and worker thread
Versioned schema migrations, role-based access, password hashing and encryption, event reporting
Door controller firmware

C STM32 FreeRTOS DeviceNet Wiegand BLE

Responsible for the firmware of a multi-mode door controller that is also driven by a site PLC.

Designed a new pneumatic door type with pressure-release valves, carried through firmware, mobile app and PC software
Found a race condition between two card readers by rebuilding the setup on the bench
Kept fail-safe, override and obstruction behaviour intact through every release
Isolated output add-on board

Altium Designer Isolation DC/DC

A plug-in board that adds two switched outputs and an extra input to an IP intercom node.

Optocoupler-isolated MOSFET outputs, each with a resettable fuse
Selected an isolated DC/DC converter so site wiring faults cannot reach the host's logic
Passed formal engineering review and went to production, with an installer wiring guide
Automated production test

C# Test design Traceability

A guided end-of-line test that runs from a PC against each unit over Ethernet.

Fixed stages covering reader, keypad, doors, lock, Bluetooth, siren, sensors, alarm I/O and memory
Drives outputs or prompts the operator, then waits for the matching input, with timeouts and retries
Saves a test record for every unit
Ethernet PHY failure investigation

Ethernet Failure analysis SMD rework

Took over a batch failure that had continued after a change of component supplier.

Measurement sequence that rules out supply, clock, reset, strapping and line-side causes one by one
Batch correlation to separate a component cause from field damage
Recommended lot traceability, incoming sample tests and a link test in production
Test jig recovery

QA Test equipment

About 2 in 5 units were failing on the production test jig.

Traced the cause to the jig's own unlabelled wiring, then rewired and labelled it against the schematics
The failures left were real soldering defects on incoming boards
Reported them with evidence, and the supplier's quality improved
Purchasing and stock system

C# SQL VBA

Rebuilt a large Excel/VBA workbook as a layered C# application.

Extracted the business rules from about 90 sheets and their macros
Added a virtual stock calculation to prevent double ordering
Verified by testing the application against the original workbook
How I work
Evidence before replacement. I form a hypothesis from the circuit or code, then prove it by measurement.
Reproduce it first. If a fault only happens on site, I build the rig that makes it happen on the bench.
Whole-system view. A fault may sit in the hardware, firmware, app or test equipment. I check all of them.
Leave a trail. Change control, test records and user documentation are part of the job.
