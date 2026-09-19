# Awesome AI Tools for Mechanical Engineering

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of AI-powered tools, copilots, and platforms for mechanical engineering — CAD, CAE/simulation, generative design, topology optimization, design review, Physics-ML surrogates, manufacturing-aware workflows, and V&V.

[日本語](README.ja.md)

## Contents

- [CAD Copilots & Text-to-CAD](#cad-copilots--text-to-cad)
- [Generative Design & Topology Optimization](#generative-design--topology-optimization)
- [Simulation, CAE & Surrogate AI](#simulation-cae--surrogate-ai)
- [Physics-ML, PINNs & Open Frameworks](#physics-ml-pinns--open-frameworks)
- [CAD Search, PDM & Knowledge](#cad-search-pdm--knowledge)
- [DFM, GD&T & Design Review](#dfm-gdt--design-review)
- [AI Tools for V&V (Verification and Validation)](#ai-tools-for-vv-verification-and-validation)
- [MCP Connectors for CAD/Design Tools](#mcp-connectors-for-caddesign-tools)
- [General Awesome Lists](#general-awesome-lists)
- [V&V Tools for Automotive Development](#vv-tools-for-automotive-development)
  - [ASAM ODS Ecosystem - Major Members & Products](#asam-ods-ecosystem---major-members--products)
  - [AI-Assisted Large-Scale V&V (Vehicle-to-Component, L0-L3)](#ai-assisted-large-scale-vv-vehicle-to-component-l0-l3)
- [Contributing](#contributing)

---

## CAD Copilots & Text-to-CAD

Natural-language assistants and text-to-CAD tools that accelerate modeling inside (or next to) MCAD.

- [SOLIDWORKS AI Virtual Companions (AURA & LEO)](https://www.solidworks.com/product/solidworks-design/ai-companions) - In-app AI companions: AURA for enterprise/web knowledge, LEO for conversational design assistance (drawings, assemblies, feature-tree help).
- [Creo AI Assistant](https://support.ptc.com/help/creo/creo_ai/usascii/ai_assistant/overview.html) - PTC's in-Creo assistant for docs, model-context Q&A, and assisted CAD tasks.
- [Autodesk Assistant in Inventor](https://help.autodesk.com/view/INVNTOR/2027/ENU/?guid=ABOUT-AUTODESK-ASSISTANT-INVENTOR) - Autodesk Assistant add-in for Inventor: natural-language help, model queries, and task automation.
- [MecAgent](https://mecagent.com/) - AI CAD copilot for SOLIDWORKS & Inventor: text-to-macros, drawing automation, engineering Q&A, and experimental text-to-STEP/STL.
- [Zoo Design Studio (Zookeeper)](https://zoo.dev/) - AI-native CAD with conversational text-to-CAD (editable B-rep / KCL); see [docs](https://zoo.dev/docs).
- [Leo AI](https://www.getleo.ai/) - Generative AI for mechanical CAD: assemblies from specs/sketches and shape-based part search.
- [CATIA / 3DEXPERIENCE](https://www.3ds.com/products/catia) - Dassault Systèmes AI capabilities for geometry assistance and platform knowledge workflows.
- [Siemens Designcenter NX AI](https://www.siemens.com/en-us/products/designcenter/cad-software/ai/) - AI-enabled NX design: command prediction, performance predictors, and generative/topology workflows.

## Generative Design & Topology Optimization

Constraint-driven geometry generation and lightweighting (loads, materials, manufacturing methods).

- [Autodesk Fusion Generative Design](https://www.autodesk.com/products/fusion-360/) - Multi-objective generative design inside Fusion (CAD/CAM/CAE), with manufacturing-aware alternatives.
- [PTC Creo Generative Design](https://www.ptc.com/en/technologies/cad/generative-design) - Creo Generative Topology Optimization (GTO) and Generative Design Extension (GDX) for constraint-driven concepts.
- [nTop](https://www.ntop.com/) - Field-driven / implicit design for lattices, topology-optimized solids, conformal channels, and AM-ready geometry (formerly nTopology).
- [Simcenter Inspire](https://www.siemens.com/en-us/products/simcenter/mechanical-simulation/inspire/) - Designer-facing topology optimization and structural concepting (OptiStruct heritage; formerly Altair Inspire).
- [Ansys GeomAI](https://www.ansys.com/products/ai/geomai) - Learns from reference geometries to explore new concepts; pairs with SimAI / solvers for performance-driven generation.
- Native CAD topology studies - Built-in lightweighting in Fusion, Creo, SOLIDWORKS Simulation, and NX Topology Optimization.

## Simulation, CAE & Surrogate AI

AI that speeds setup, explores designs in real time, or predicts fields from past CAE data.

- [Ansys SimAI](https://www.ansys.com/products/ai/simai) - Train AI models on legacy simulation results to predict 3D fields for new designs (SimAI Pro desktop / Premium cloud).
- [Ansys Discovery](https://www.ansys.com/products/3d-design/ansys-discovery) - Real-time structural / thermal / fluid exploration on the GPU, with handoff to Fluent and other flagship solvers.
- [Simcenter PhysicsAI](https://www.siemens.com/en-us/products/simcenter/engineering-data-science-ai/physicsai/) - Geometric deep learning on CAE data for fast physics predictions across meshes/topologies (ex-Altair PhysicsAI).
- [Neural Concept](https://www.neuralconcept.com/) - Geometry-aware AI for real-time multiphysics prediction and design-space exploration (strong in aero / thermal use cases).
- [SimScale](https://www.simscale.com/) - Cloud CAE (FEA/CFD/thermal) with AI-assisted setup and collaboration for design engineers.

## Physics-ML, PINNs & Open Frameworks

Open frameworks for physics-informed and data-driven surrogates — useful when you own the training loop.

- [NVIDIA PhysicsNeMo](https://developer.nvidia.com/physicsnemo) - <span style="color:blue">Open PyTorch framework for PINNs, neural operators, GNNs, and hybrid Physics-ML (CFD, structural, EM examples). (Open source)</span> — [GitHub](https://github.com/NVIDIA/physicsnemo)
- [DeepXDE](https://deepxde.readthedocs.io/) - <span style="color:blue">Popular library for PINNs and deep learning for PDEs; good teaching / research entry point. (Open source)</span> — [GitHub](https://github.com/lululxvi/deepxde)

## CAD Search, PDM & Knowledge

Reuse validated parts and tribal knowledge instead of reinventing geometry.

- [Leo AI](https://www.getleo.ai/) - Finds geometrically similar parts in your vault/PDM by shape, not only by name or part number.
- [SOLIDWORKS AURA](https://www.solidworks.com/product/solidworks-design/ai-companions) - Connects designers to company knowledge, 3DSwym content, and documentation inside the design environment.

## DFM, GD&T & Design Review

Automated drawing/model review, change detection, and manufacturability checks.

- [bananaz](https://www.bananaz.ai/) - AI agents for mechanical design review: CAD/drawing revision diffs, DFM checks, GD&T/tolerance review, and redlines.
- [CoLab AutoReview](https://www.colabsoftware.com/product/autoreview) - AI design reviews on models and drawings (GD&T, completeness, standards, process-specific DFM) with tracked markups.

## AI Tools for V&V (Verification and Validation)

ML and SPDM that reduce physical prototypes and keep simulation evidence traceable.

- [Monolith AI](https://www.monolithai.com/) - Machine learning for virtual testing: predict outcomes from past tests/sims and cut physical prototype loops.
- [Ansys Minerva](https://www.ansys.com/products/connect/ansys-minerva) - Simulation process & data management (SPDM) for traceable, auditable V&V workflows.
- [Siemens Simcenter Testlab](https://www.siemens.com/en-us/products/simcenter/physical-testing/testlab/) - Physical testing / NVH analytics with correlation paths from test data back to simulation models.
- [COMSOL Model Manager](https://www.comsol.com/model-manager) - Manages, verifies, and version-controls multiphysics models across the V&V lifecycle.

## MCP Connectors for CAD/Design Tools

Model Context Protocol servers that let AI agents talk to CAD/design apps.

- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) - <span style="color:blue">Curated list including MCP connectors for CAD/design vendors (e.g. Autodesk Fusion MCP / Data MCP, Blender Lab MCP, SketchUp Connector). (Open source)</span>

## General Awesome Lists

- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) - <span style="color:blue">AI tools for hardware engineering — CAD, simulation, manufacturing, and beyond. (Open source)</span>
- [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) - <span style="color:blue">AI-callable CAE/CAD tooling and related resources. (Open source)</span>
- [awesome-cad-cae](https://github.com/shvyac/awesome-cad-cae) - <span style="color:blue">CAD/CAE apps, kernels, FEA/CFD, topology optimization, and TAC tooling. (Open source)</span>
- [awesome-mechanical-engineering](https://github.com/awesomelistsio/awesome-mechanical-engineering) - <span style="color:blue">Broader mechanical-engineering tools, platforms, and learning resources. (Open source)</span>

## V&V Tools for Automotive Development

- [dSPACE SCALEXIO / ASM](https://www.dspace.com/) - Hardware-in-the-loop (HIL) test systems and simulation models for verifying ECU software and vehicle dynamics.
- [Vector CANoe](https://www.vector.com/int/en/products/products-a-z/software/canoe/) - Tool for development, testing, and analysis of ECUs and networks across the automotive V-model.
- [National Instruments VeriStand](https://www.ni.com/en/shop/veristand.html) - Real-time testing software for HIL simulation, model validation, and rapid control prototyping.
- [MathWorks Simulink Test & Requirements Toolbox](https://www.mathworks.com/products/simulink-test.html) - Manages requirements traceability and automates verification of Simulink models against test cases.
- [ETAS LABCAR](https://www.etas.com/en/products/labcar.php) - HIL test environment for validating automotive ECUs under realistic operating conditions.
- [ASAM ODS (Open Data Services)](https://www.asam.net/standards/detail/ods/) - European standard for test data management, storing and exchanging measurement, simulation, and validation results across the V-model.

#### ASAM ODS Ecosystem - Major Members & Products

Major ASAM e.V. member companies that develop and maintain ASAM ODS-based test data management products.

- [Peak Solution](https://www.peak-solution.com/) - Active contributor to the ASAM ODS working group; develops the [Peak ODS Server (PODS)](https://www.asam.net/members/product-directory/detail/peak-ods-server/), a platform-independent ASAM ODS server, and is a lead contributor to openMDM.
- [AVL](https://www.avl.com/) - OEM/Tier-1 test equipment supplier whose [AVL CONCERTO](https://www.avl.com/) data analysis platform supports ASAM ODS for managing powertrain and vehicle test data.
- [Vector Informatik](https://www.vector.com/) - ASAM member providing measurement and calibration tools (e.g., CANape, vSignalyzer) with ASAM ODS-based data management and exchange.
- [Robert Bosch GmbH](https://www.bosch.com/) - OEM/Tier-1 ASAM member contributing requirements and use cases for ASAM ODS in automotive test data management.
- [HighQSoft](https://www.highqsoft.com/) - ASAM member offering ASAM ODS consulting, data model design, and integration services for test data management systems.
- [MBBM-VAS](https://www.mbbm-vas.com/) - ASAM member providing [ASAM ODS & openMDM-based](https://www.mbbm-vas.com/en/products/data-management/asam-ods) data management products for measurement and test data.

### AI-Assisted Large-Scale V&V (Vehicle-to-Component, L0-L3)

Tools that support the full automotive V-model: left-side requirements decomposition from whole-vehicle (L0) down to systems (L1), subsystems (L2), and components/parts (L3), and right-side validation that rolls component-level (L3) test results back up to whole-vehicle (L0) validation.

- [Siemens Polarion + Capital](https://www.plm.automation.siemens.com/global/en/products/polarion/) - AI-assisted requirements management and impact analysis with end-to-end traceability across vehicle, system, subsystem, and component levels.
- [PTC Codebeamer X](https://www.ptc.com/en/products/codebeamer) - AI-powered requirements decomposition, coverage analysis, and test traceability across the full V-model hierarchy.
- [Vector PREEvision](https://www.vector.com/int/en/products/products-a-z/software/preevision/) - E/E systems engineering tool for decomposing vehicle-level requirements into system, subsystem, and component specifications, with traceability for V&V roll-up.
- [IBM Engineering Lifecycle Management (ELM) with watsonx](https://www.ibm.com/products/engineering-lifecycle-management) - AI-assisted requirements analysis, change impact, and verification traceability spanning vehicle to part-level artifacts.
- [Ansys medini analyze](https://www.ansys.com/products/safety-analysis/ansys-medini-analyze) - Model-based safety and requirements analysis that links system-level hazards to component-level verification evidence.

#### Open Source Alternatives

Open-source projects targeting the same vehicle-to-component V-model decomposition and validation roll-up goals.

- [Eclipse Capella](https://github.com/eclipse-capella/capella) - <span style="color:blue">Open-source MBSE tool implementing the Arcadia method for decomposing system architectures across operational, system, logical, and physical levels (L0-L3). (Open source)</span>
- [Eclipse SCORE](https://github.com/eclipse-score/score) - <span style="color:blue">Bosch-led open-source platform for software-defined vehicles, including requirements, architecture, and V&V tooling across the vehicle software stack. (Open source)</span>
- [OpenMBEE](https://github.com/Open-MBEE) - <span style="color:blue">NASA JPL's open-source model-based systems engineering environment for managing requirements and architecture traceability from system to component level. (Open source)</span>
- [Eclipse ProR](https://github.com/eclipse-rmf/org.eclipse.rmf) - <span style="color:blue">Open-source ReqIF-based requirements management and traceability tool for linking requirements across system levels to verification artifacts. (Open source)</span>
- [CARLA](https://github.com/carla-simulator/carla) + [ASAM OpenSCENARIO/OpenDRIVE](https://github.com/esmini/esmini) - <span style="color:blue">Open-source autonomous-driving simulator and scenario standards for rolling up component/scenario-level test results into whole-vehicle validation. (Open source)</span>
- [openMDM](https://openmdm.org/) - <span style="color:blue">Eclipse Foundation open-source kit of components and concepts, built on the ASAM ODS standard, for composing measured/test data management systems used to exchange and trace test and validation data across the V-model. (Open source)</span>

## Contributing

Contributions welcome! Please open a pull request to add a tool, fix a broken link, or suggest a new category.

Prefer **durable official / docs URLs**, short blurbs, and tools that are shipping (not vaporware). Mark open-source entries clearly.

## License

See [LICENSE](LICENSE).
