# Suleman Ali

M.Sc. student in Electrical Engineering and Information Technology at Otto von Guericke University Magdeburg, Germany.

I build reusable automation software, and I commission the machines it runs on. Frameworks and standard blocks on the PLC, and tools on the PC that read, test and connect it. Before my Master's I spent a year commissioning automation systems for packaging, food and manufacturing plants: adapting PLC programs, integrating HMI/SCADA over PROFINET and OPC UA, and getting stopped lines running again.

How I build: every repo has tests that run in CI, a README that states its limits, and numbers traced to a measurement or a standard.

- **PLC:** Siemens S7-1200 / S7-1500 (TIA Portal), Beckhoff TwinCAT 3, IEC 61131-3 (LAD, FBD, ST/SCL)
- **Integration:** OPC UA (information models, security), Asset Administration Shell (IDTA submodels, Eclipse BaSyx), PROFINET, MQTT, Beckhoff ADS
- **Software:** Python, ROS 2, Git, CI with GitHub Actions
- **Electrical:** EPLAN Electric P8, drives and VFDs, cabinet testing

## Libraries and tools

Things made to be reused on the next machine.

| Project | What it does |
|---|---|
| [aidconnect](https://github.com/sulemanali5760/aidconnect) | Python library: connects to an OPC UA asset from its Asset Administration Shell alone. Endpoint, security and datapoints come from the Asset Interfaces Description; includes a gateway that publishes live values on the AAS REST API |
| [twincat3-pickplace-framework](https://github.com/sulemanali5760/twincat3-pickplace-framework) | Minimal machine framework in TwinCAT 3 Structured Text: node tree, mode handling, pick-and-place unit running on a soft-PLC |
| [opcua-tagmap](https://github.com/sulemanali5760/opcua-tagmap) | Command-line tool: browses an OPC UA server and generates collector configs and tag inventories |
| [opc-ua-test-automation-pipeline](https://github.com/sulemanali5760/opc-ua-test-automation-pipeline) | Reads live PLC data over OPC UA or ADS, checks it against a written test case and generates a pass/fail report |

## Plants and systems

Complete applications, commissioned in simulation.

| Project | What it does |
|---|---|
| [heating-plant-aas](https://github.com/sulemanali5760/heating-plant-aas) | A commissioned S7-1500 heating plant as an Industrie 4.0 component: Python model checked sample by sample against the PLCSIM trace, controller robustness analysis (stability margins, valve actuator, sensor noise), secured OPC UA server with a typed model, Asset Administration Shell from official IDTA templates, AAS REST API |
| [twincat3-hrl-virtual-commissioning](https://github.com/sulemanali5760/twincat3-hrl-virtual-commissioning) | Virtual commissioning of a pallet high-bay warehouse in TwinCAT 3: stacker crane, conveyor standard block, telegram interface to the material flow computer, 37 TcUnit tests |
| [amr-station-handshake](https://github.com/sulemanali5760/amr-station-handshake) | A mobile robot hands a load to a PLC-controlled conveyor station: ROS 2 action on the robot side, OPC UA signal handshake with per-phase timeouts on the PLC side |

## Contact

[LinkedIn](https://www.linkedin.com/in/suleman-ali-5760) · [Portfolio](https://sulemanali.store)

Open to working student positions in PLC programming and industrial automation in Germany. Willing to relocate.

Offen für Werkstudentenstellen in SPS-Programmierung und Automatisierungstechnik, deutschlandweit und umzugsbereit.
