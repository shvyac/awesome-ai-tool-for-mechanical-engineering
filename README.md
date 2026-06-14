# Awesome AI Tools for Mechanical Engineering

A curated list of AI-powered tools, copilots, and platforms for mechanical engineering — covering CAD, simulation, generative design, topology optimization, manufacturing, and more.

[日本語](README.ja.md)

## Contents

- [CAD Copilots & Generative Design](#cad-copilots--generative-design)
- [Simulation & CAE (FEA/CFD)](#simulation--cae-feacfd)
- [Topology Optimization & Lightweighting](#topology-optimization--lightweighting)
- [CAD Search, PDM & Knowledge](#cad-search-pdm--knowledge)
- [DFM, GD&T & Design Review](#dfm-gdt--design-review)
- [AI Tools for V&V (Verification and Validation)](#ai-tools-for-vv-verification-and-validation)
- [MCP Connectors for CAD/Design Tools](#mcp-connectors-for-caddesign-tools)
- [General Awesome Lists](#general-awesome-lists)
- [V&V Tools for Automotive Development](#vv-tools-for-automotive-development)
  - [AI-Assisted Large-Scale V&V (Vehicle-to-Component, L0-L3)](#ai-assisted-large-scale-vv-vehicle-to-component-l0-l3)
- [Contributing](#contributing)

## CAD Copilots & Generative Design

- [SolidWorks AURA](https://www.solidworks.com/) - AI assistant integrated into SolidWorks for design automation and command prediction.
- [Creo AI Assistant](https://www.ptc.com/en/products/creo) - PTC's AI assistant for Creo offering geometry generation and modeling guidance.
- [Inventor Design Copilot](https://www.autodesk.com/products/inventor/) - AI-driven design assistant for Autodesk Inventor.
- [CATIA 3DEXPERIENCE AI](https://www.3ds.com/products/catia) - Dassault Systèmes' AI capabilities for geometry generation and constraint automation.
- [Fusion 360 Generative Design](https://www.autodesk.com/products/fusion-360/) - Generates optimized design alternatives based on constraints and manufacturing methods.
- [Leo AI](https://www.getleo.ai/) - Generative AI for engineering CAD design and shape-based part search.

## Simulation & CAE (FEA/CFD)

- [Ansys AI+](https://www.ansys.com/) - AI-assisted FEA/CFD setup, meshing, and boundary condition suggestions.
- [SimScale](https://www.simscale.com/) - Cloud-based CAE platform with AI-assisted simulation setup for FEA, CFD, and thermal analysis.
- [Autodesk Discovery](https://www.autodesk.com/) - Real-time simulation feedback (structural, thermal, fluid flow) during modeling, without long solve times.

## Topology Optimization & Lightweighting

- [nTopology](https://ntopology.com/) - Engineering design software for topology optimization, lattice structures, and generative geometry.
- Native CAD topology optimization tools (Fusion 360, Creo, SolidWorks) - Built-in generative geometry and weight-reduction features.

## CAD Search, PDM & Knowledge

- [Leo AI](https://www.getleo.ai/) - Finds geometrically similar parts in your PDM by shape rather than name or part number.

## DFM, GD&T & Design Review

- [bananaz](https://www.bananaz.ai/) - Detects geometric changes between CAD revisions and automates DFM checks, GD&T, tolerance analysis, and design inspections.

## AI Tools for V&V (Verification and Validation)

- [Monolith AI](https://monolithai.com/) - Machine learning platform for virtual testing that predicts test outcomes and helps validate designs with fewer physical prototypes.
- [Ansys minerva](https://www.ansys.com/products/digital-twin/ansys-minerva) - AI-assisted simulation process and data management for traceable, auditable verification and validation workflows.
- [Siemens Simcenter Testlab](https://www.plm.automation.siemens.com/global/en/products/simcenter/simcenter-testlab.html) - AI-driven test data analytics that correlate physical test results with simulation models for validation.
- [COMSOL Model Manager](https://www.comsol.com/) - Manages, verifies, and version-controls multiphysics simulation models throughout the V&V process.

## MCP Connectors for CAD/Design Tools

- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/awesome-engineering-ai) - <span style="color:blue">Curated list including official MCP connectors for CAD/design vendors: Autodesk Fusion MCP, Autodesk Fusion Data MCP, the Blender Lab MCP server, and the SketchUp Connector. (Open source)</span>

## General Awesome Lists

- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/awesome-engineering-ai) - <span style="color:blue">A curated list of AI tools for hardware engineering — CAD, simulation, manufacturing, and beyond. (Open source)</span>
- [awesome-mechanical-engineering](https://github.com/awesomelistsio/awesome-mechanical-engineering) - <span style="color:blue">A curated list of tools, platforms, resources, and educational content for Mechanical Engineering. (Open source)</span>

## V&V Tools for Automotive Development

- [dSPACE SCALEXIO / ASM](https://www.dspace.com/) - Hardware-in-the-loop (HIL) test systems and simulation models for verifying ECU software and vehicle dynamics.
- [Vector CANoe](https://www.vector.com/int/en/products/products-a-z/software/canoe/) - Tool for development, testing, and analysis of ECUs and networks across the automotive V-model.
- [National Instruments VeriStand](https://www.ni.com/en/shop/veristand.html) - Real-time testing software for HIL simulation, model validation, and rapid control prototyping.
- [MathWorks Simulink Test & Requirements Toolbox](https://www.mathworks.com/products/simulink-test.html) - Manages requirements traceability and automates verification of Simulink models against test cases.
- [ETAS LABCAR](https://www.etas.com/en/products/labcar.php) - HIL test environment for validating automotive ECUs under realistic operating conditions.

### AI-Assisted Large-Scale V&V (Vehicle-to-Component, L0-L3)

Tools that support the full automotive V-model: left-side requirements decomposition from whole-vehicle (L0) down to systems (L1), subsystems (L2), and components/parts (L3), and right-side validation that rolls component-level (L3) test results back up to whole-vehicle (L0) validation.

- [Siemens Polarion + Capital](https://www.plm.automation.siemens.com/global/en/products/polarion/) - AI-assisted requirements management and impact analysis with end-to-end traceability across vehicle, system, subsystem, and component levels.
- [PTC Codebeamer X](https://www.ptc.com/en/products/codebeamer) - AI-powered requirements decomposition, coverage analysis, and test traceability across the full V-model hierarchy.
- [Vector PREEvision](https://www.vector.com/int/en/products/products-a-z/software/preevision/) - E/E systems engineering tool for decomposing vehicle-level requirements into system, subsystem, and component specifications, with traceability for V&V roll-up.
- [IBM Engineering Lifecycle Management (ELM) with watsonx](https://www.ibm.com/products/engineering-lifecycle-management) - AI-assisted requirements analysis, change impact, and verification traceability spanning vehicle to part-level artifacts.
- [Ansys medini analyze](https://www.ansys.com/products/safety-analysis/ansys-medini-analyze) - Model-based safety and requirements analysis that links system-level hazards to component-level verification evidence.


## Contributing

Contributions welcome! Please open a pull request to add a tool, fix a broken link, or suggest a new category.

## License

See [LICENSE](LICENSE).
