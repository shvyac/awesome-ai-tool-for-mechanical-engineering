# Awesome AI Tools for Mechanical Engineering

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

**AI copilots and platforms for the mechanical workflow** — commercial CAD assistants, generative design, CAE surrogates, DFM review, and V&V — not only agent-callable OSS.

**Scope:** commercial + open tools across **CAD → CAE → review → V&V** for mechanical engineers.

⭐ badges show live GitHub star counts (via shields.io). Release badges show the latest GitHub release version and date.

[日本語](README.ja.md)

## Start here

| I want to… | Go to |
| --- | --- |
| Speed up modeling in CAD | [CAD Copilots & Text-to-CAD](#cad-copilots--text-to-cad) |
| Explore shapes / lightweight | [Generative Design & Topology Optimization](#generative-design--topology-optimization) |
| Faster what-if physics | [Simulation, CAE & Surrogate AI](#simulation-cae--surrogate-ai) |
| Train my own Physics-ML | [Physics-ML, PINNs & Open Frameworks](#physics-ml-pinns--open-frameworks) |
| Reuse parts / knowledge | [CAD Search, PDM & Knowledge](#cad-search-pdm--knowledge) |
| Check drawings / DFM | [DFM, GD&T & Design Review](#dfm-gdt--design-review) |
| Trace tests & sims | [V&V (Verification & Validation)](#vv-verification--validation) |
| Agent / MCP connectors | [MCP & Agent Tooling](#mcp--agent-tooling) |

## Contents

- [CAD Copilots & Text-to-CAD](#cad-copilots--text-to-cad)
- [Generative Design & Topology Optimization](#generative-design--topology-optimization)
- [Simulation, CAE & Surrogate AI](#simulation-cae--surrogate-ai)
- [Physics-ML, PINNs & Open Frameworks](#physics-ml-pinns--open-frameworks)
- [CAD Search, PDM & Knowledge](#cad-search-pdm--knowledge)
- [DFM, GD&T & Design Review](#dfm-gdt--design-review)
- [V&V (Verification & Validation)](#vv-verification--validation)
- [MCP & Agent Tooling](#mcp--agent-tooling)
- [Related Awesome Lists](#related-awesome-lists)
- [Automotive V&V (deep-dive)](#automotive-vv-deep-dive)
- [Contributing](#contributing)
- [License](#license)
- [shvyac's awesome lists](#shvyacs-awesome-lists)

---

## CAD Copilots & Text-to-CAD

Natural-language assistants and text-to-CAD that accelerate modeling inside (or next to) MCAD.

- [SOLIDWORKS AI Virtual Companions (AURA, LEO & MARIE)](https://www.solidworks.com/product/solidworks-design/ai-virtual-companions) — In-app companions: AURA for enterprise/web knowledge, LEO for conversational design help, MARIE for materials guidance. Tags: `Commercial`
- [Creo AI Assistant](https://support.ptc.com/help/creo/creo_ai/usascii/ai_assistant/overview.html) — In-Creo agents: Creo Advise (free docs and model-context Q&A) and Creo Assist (assisted CAD tasks, Advanced AI license). Tags: `Commercial`
- [Autodesk Assistant in Inventor](https://www.autodesk.com/blogs/design-and-manufacturing/meet-autodesk-assistant-in-inventor-2027/) — Natural-language help, model queries, and task automation in Inventor (since Inventor 2027). Tags: `Commercial`
- [MecAgent](https://mecagent.com/) — SOLIDWORKS & Inventor copilot plus the V2 in-SOLIDWORKS agent: text/image-to-CAD, drawing-to-CAD, assemblies, BOMs, macros and drawings (Onshape version planned). Tags: `Commercial`
- [Zoo Design Studio](https://zoo.dev/) — AI-native CAD with the Zookeeper agent for conversational text-to-CAD (editable B-rep / KCL). Tags: `Commercial`
- [Leo AI](https://www.getleo.ai/) — Spec/sketch → assemblies plus shape-based part search across your vault. Tags: `Commercial`
- [Adam](https://adam.new/) — AI CAD copilot for hardware teams (YC): ask in Slack or email and get model edits on a branch, BOMs, drawings, and supplier quotes across Onshape, Fusion, and SOLIDWORKS. Tags: `Commercial`
- [CATIA / 3DEXPERIENCE](https://www.3ds.com/products/catia) — Dassault AI for geometry assistance and platform knowledge workflows. Tags: `Commercial`
- [Siemens NX AI](https://www.siemens.com/en-us/products/designcenter/cad-software/ai/) — Command prediction, performance predictors, and generative/topology workflows in NX (now part of Siemens Designcenter). Tags: `Commercial`

## Generative Design & Topology Optimization

Constraint-driven geometry and lightweighting (loads, materials, manufacturing methods).

- [Autodesk Fusion Generative Design](https://www.autodesk.com/products/fusion-360/) — Multi-objective generative design in Autodesk Fusion (formerly Fusion 360) with manufacturing-aware alternatives. Tags: `Commercial`
- [PTC Creo Generative Design](https://www.ptc.com/en/technologies/cad/generative-design) — Creo GTO / GDX for constraint-driven concept exploration. Tags: `Commercial`
- [nTop](https://www.ntop.com/) — Field-driven / implicit design for lattices, topology solids, conformal channels, AM-ready geometry. Tags: `Commercial`
- [Simcenter Inspire](https://www.siemens.com/en-us/products/simcenter/mechanical-simulation/inspire/) — Designer-facing topology optimization and structural concepting (formerly Altair Inspire, now in the Simcenter family). Tags: `Commercial`
- [Ansys GeomAI](https://ansys.synopsys.com/products/ai/geomai) — Learns from reference geometries to explore concepts; pairs with SimAI / solvers (Ansys is now part of Synopsys). Tags: `Commercial`
- Native CAD topology studies — Built-in lightweighting in Fusion, Creo, SOLIDWORKS Simulation, and NX Topology Optimization. Tags: `Commercial`

## Simulation, CAE & Surrogate AI

Faster setup, real-time what-if exploration, or field prediction from past CAE data.

- [AgentFEM](https://haoming-luo.github.io/agentfem/) — AI-agent-ready finite-element workflows with editable Python models, pre-run checks, numerical solves, and inspectable results, using a local FEniCSx-based runtime ([GitHub](https://github.com/haoming-luo/agentfem)). Tags: `OSS`
- [Ansys SimAI](https://www.ansys.com/products/ai/simai) — Train on legacy simulation results to predict 3D fields for new designs; offered as SimAI Pro and SimAI Premium. Tags: `Commercial`
- [Ansys Discovery](https://ansys.synopsys.com/products/3d-design/ansys-discovery) — Real-time structural / thermal / fluid exploration on GPU, with handoff to flagship solvers (Ansys is now part of Synopsys). Tags: `Commercial`
- [Simcenter PhysicsAI](https://www.siemens.com/en-us/products/simcenter/engineering-data-science-ai/physicsai/) — Geometric deep learning on CAE data for fast physics across meshes/topologies. Tags: `Commercial`
- [Neural Concept](https://www.neuralconcept.com/) — Geometry-aware AI for real-time multiphysics prediction and design-space exploration. Tags: `Commercial`
- [PhysicsX](https://www.physicsx.ai/) — AI-native engineering stack combining simulation, physics AI, and data across design, manufacturing, and operations. Tags: `Commercial`
- [Luminary](https://luminary.ai/) — Physics AI platform (formerly Luminary Cloud) for training and deploying "Large Physics Models" that predict flow, structures, and heat in under a second. Tags: `Commercial`
- [SimScale](https://www.simscale.com/) — Cloud FEA/CFD/thermal with AI-assisted setup and collaboration. Tags: `Commercial`

## Physics-ML, PINNs & Open Frameworks

Open stacks when you own the training loop (PINNs, neural operators, hybrid Physics-ML).

- [NVIDIA PhysicsNeMo](https://developer.nvidia.com/physicsnemo) ![GitHub stars](https://img.shields.io/github/stars/NVIDIA/physicsnemo?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/NVIDIA/physicsnemo?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/NVIDIA/physicsnemo?style=flat&label=released) — PyTorch framework for PINNs, neural operators, GNNs, and hybrid Physics-ML ([GitHub](https://github.com/NVIDIA/physicsnemo)). Tags: `OSS`
- [DeepXDE](https://deepxde.readthedocs.io/) ![GitHub stars](https://img.shields.io/github/stars/lululxvi/deepxde?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/lululxvi/deepxde?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/lululxvi/deepxde?style=flat&label=released) — Popular PINNs / deep-learning-for-PDEs library; strong teaching entry point ([GitHub](https://github.com/lululxvi/deepxde)). Tags: `OSS`

## CAD Search, PDM & Knowledge

Reuse validated parts and tribal knowledge instead of reinventing geometry.

- [SOLIDWORKS AURA](https://www.solidworks.com/product/solidworks-design/ai-virtual-companions) — Connects designers to company knowledge, 3DSwym, and docs inside the design environment. Tags: `Commercial`
- See also [Leo AI](#cad-copilots--text-to-cad) for shape-based similar-part search in vaults/PDM.

## DFM, GD&T & Design Review

Automated drawing/model review, change detection, and manufacturability checks.

- [bananaz](https://www.bananaz.ai/) — AI agents for CAD/drawing diffs, DFM, GD&T/tolerance review, and redlines. Tags: `Commercial`
- [CoLab AutoReview](https://www.colabsoftware.com/product/autoreview) — AI reviews on models and drawings (GD&T, completeness, standards, DFM) with tracked markups; rolling out to early customers (waitlist). Tags: `Commercial`

## V&V (Verification & Validation)

ML and SPDM that cut physical prototypes and keep simulation evidence traceable.

- [Monolith](https://www.monolithai.com/) — ML for virtual testing: predict outcomes from past tests/sims and shrink prototype loops (now part of CoreWeave). Tags: `Commercial`
- [Ansys Minerva](https://ansys.synopsys.com/products/connect/ansys-minerva) — SPDM (powered by Aras) for traceable, auditable simulation V&V workflows. Tags: `Commercial`
- [Siemens Simcenter Testlab](https://www.siemens.com/en-us/products/simcenter/physical-testing/testlab/) — Physical testing / NVH analytics with test↔simulation correlation. Tags: `Commercial`
- [COMSOL Model Manager](https://www.comsol.com/comsol-multiphysics/model-manager) — Version-control and verify multiphysics models across the V&V lifecycle. Tags: `Commercial`

## MCP & Agent Tooling

Brief pointers for agents that talk to CAD/CAE apps. This list stays **ME-workflow first** (including commercial tools); for OSS agent-callability rankings, see [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae).

- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) ![GitHub stars](https://img.shields.io/github/stars/010zx00x1/Awesome-Physical-Engineering-AI?style=flat&label=%E2%AD%90) — Curated MCP connectors and AI tooling for CAD/design (e.g. Fusion MCP, Blender Lab MCP, SketchUp). Tags: `OSS`
- [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) ![GitHub stars](https://img.shields.io/github/stars/kimimgo/awesome-ai-cae?style=flat&label=%E2%AD%90) — Agent-callable OSS CAE/CAD stack (MCP / Python / CLI), with readiness ranking. Tags: `OSS`
- [Autodesk Fusion MCP](https://www.autodesk.com/products/fusion-360/blog/introducing-the-fusion-mcp-opening-fusion-to-ai-powered-workflows/) — Official MCP servers that let AI clients create and edit designs inside Fusion (desktop) and work with Fusion project data (Fusion Data MCP Server). Tags: `Commercial`
- [Onshape FeatureScript MCP Server](https://www.onshape.com/en/features/onshape-labs) — Onshape Labs (PTC) early-access server: AI clients write, run, and fix FeatureScript to build reusable parametric custom features. Tags: `Commercial`
- [text-to-cad](https://github.com/earthtojake/text-to-cad) ![GitHub stars](https://img.shields.io/github/stars/earthtojake/text-to-cad?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/earthtojake/text-to-cad?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/earthtojake/text-to-cad?style=flat&label=released) — Open-source agent toolkit that gives AI coding agents CAD abilities (STEP/STL output); trending on GitHub in Oct 2026. Tags: `OSS`

## Related Awesome Lists

- [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) ![GitHub stars](https://img.shields.io/github/stars/kimimgo/awesome-ai-cae?style=flat&label=%E2%AD%90) — AI-callable CAE/CAD tooling and agent readiness. Tags: `OSS`
- [awesome-cad-cae](https://github.com/shvyac/awesome-cad-cae) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-cad-cae?style=flat&label=%E2%AD%90) — CAD/CAE apps, kernels, FEA/CFD, topology optimization. Tags: `OSS`
- [awesome-open-source-solvers](https://github.com/shvyac/awesome-open-source-solvers) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-open-source-solvers?style=flat&label=%E2%AD%90) — Open FEM/CFD/MBD/particle solvers and scientific stacks. Tags: `OSS`
- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) ![GitHub stars](https://img.shields.io/github/stars/010zx00x1/Awesome-Physical-Engineering-AI?style=flat&label=%E2%AD%90) — Broader hardware-engineering AI (CAD, sim, manufacturing). Tags: `OSS`
- [awesome-mechanical-engineering](https://github.com/brandonhimpfen/awesome-mechanical-engineering) ![GitHub stars](https://img.shields.io/github/stars/brandonhimpfen/awesome-mechanical-engineering?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/brandonhimpfen/awesome-mechanical-engineering?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/brandonhimpfen/awesome-mechanical-engineering?style=flat&label=released) — Broader ME tools, platforms, and learning resources. Tags: `OSS`

## Automotive V&V (deep-dive)

Optional short list for vehicle HIL / ECU V&V. Skip unless you work automotive control & test.

### HIL & test tooling

- [dSPACE SCALEXIO / ASM](https://www.dspace.com/) — HIL systems and vehicle/ECU simulation models. Tags: `Commercial`
- [Vector CANoe](https://www.vector.com/en/product/canoe/) — ECU & network development, testing, and analysis (SIL & HIL). Tags: `Commercial`
- [NI VeriStand](https://www.ni.com/en-us/shop/product/veristand.html) — Real-time HIL, model validation, and rapid control prototyping (NI is now part of Emerson). Tags: `Commercial`
- [MathWorks Simulink Test](https://www.mathworks.com/products/simulink-test.html) — Requirements traceability and automated model verification. Tags: `Commercial`
- [ETAS LABCAR](https://www.etas.com/ww/en/products-services/) — HIL environment for ECU validation under realistic conditions. Tags: `Commercial`
- [ASAM ODS](https://www.asam.net/standards/detail/ods/) — Standard for exchanging measurement, simulation, and validation data. Tags: `Commercial`

Pointers into the ODS ecosystem (not a full vendor catalog): [Peak ODS Server](https://www.peak-solution.com/), [openMDM](https://openmdm.org/), [AVL CONCERTO](https://www.avl.com/).

### Open-source MBSE / scenario (few)

- [Eclipse Capella](https://github.com/eclipse-capella/capella) ![GitHub stars](https://img.shields.io/github/stars/eclipse-capella/capella?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/eclipse-capella/capella?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/eclipse-capella/capella?style=flat&label=released) — Arcadia MBSE for architecture decomposition across system levels. Tags: `OSS`
- [CARLA](https://github.com/carla-simulator/carla) ![GitHub stars](https://img.shields.io/github/stars/carla-simulator/carla?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/carla-simulator/carla?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/carla-simulator/carla?style=flat&label=released) + [esmini / OpenSCENARIO](https://github.com/esmini/esmini) ![GitHub stars](https://img.shields.io/github/stars/esmini/esmini?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/esmini/esmini?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/esmini/esmini?style=flat&label=released) — Open driving simulator and scenario standards for scenario-level V&V. Tags: `OSS`
- [openMDM](https://openmdm.org/) — Eclipse components for ASAM ODS–based test data management (the Eclipse working group is no longer active). Tags: `OSS`

## Contributing

Contributions welcome — open a PR to add a tool, fix a link, or suggest a category.

Prefer **durable official / docs URLs**, one crisp sentence, and tools that are shipping. Tag each entry `Commercial` or `OSS`. Keep EN and JA READMEs in sync.

## License

See [LICENSE](LICENSE).

## shvyac's awesome lists

All curated lists maintained by [shvyac](https://github.com/shvyac):

- [awesome-AI-Powered-Executive-Dashboards](https://github.com/shvyac/awesome-AI-Powered-Executive-Dashboards) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-AI-Powered-Executive-Dashboards?style=flat&label=%E2%AD%90)
- [awesome-ai-tool-for-mechanical-engineering](https://github.com/shvyac/awesome-ai-tool-for-mechanical-engineering) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-ai-tool-for-mechanical-engineering?style=flat&label=%E2%AD%90)
- [awesome-audio-softwares](https://github.com/shvyac/awesome-audio-softwares) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-audio-softwares?style=flat&label=%E2%AD%90)
- [awesome-azure-ai-dynamics365-security](https://github.com/shvyac/awesome-azure-ai-dynamics365-security) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-azure-ai-dynamics365-security?style=flat&label=%E2%AD%90)
- [awesome-ballroom-dance](https://github.com/shvyac/awesome-ballroom-dance) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-ballroom-dance?style=flat&label=%E2%AD%90)
- [awesome-cad-cae](https://github.com/shvyac/awesome-cad-cae) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-cad-cae?style=flat&label=%E2%AD%90)
- [awesome-cms-ai](https://github.com/shvyac/awesome-cms-ai) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-cms-ai?style=flat&label=%E2%AD%90)
- [awesome-dashboards-visualization](https://github.com/shvyac/awesome-dashboards-visualization) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-dashboards-visualization?style=flat&label=%E2%AD%90)
- [awesome-ghost-artists](https://github.com/shvyac/awesome-ghost-artists) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-ghost-artists?style=flat&label=%E2%AD%90)
- [awesome-hamradio](https://github.com/shvyac/awesome-hamradio) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-hamradio?style=flat&label=%E2%AD%90)
- [awesome-hpc](https://github.com/shvyac/awesome-hpc) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-hpc?style=flat&label=%E2%AD%90)
- [awesome-iso27001-isms-tools](https://github.com/shvyac/awesome-iso27001-isms-tools) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-iso27001-isms-tools?style=flat&label=%E2%AD%90)
- [awesome-local-llm](https://github.com/shvyac/awesome-local-llm) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-local-llm?style=flat&label=%E2%AD%90)
- [awesome-m5stack-arduino](https://github.com/shvyac/awesome-m5stack-arduino) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-m5stack-arduino?style=flat&label=%E2%AD%90)
- [awesome-map-gis](https://github.com/shvyac/awesome-map-gis) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-map-gis?style=flat&label=%E2%AD%90)
- [awesome-meshless-cae](https://github.com/shvyac/awesome-meshless-cae) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-meshless-cae?style=flat&label=%E2%AD%90)
- [awesome-online-services](https://github.com/shvyac/awesome-online-services) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-online-services?style=flat&label=%E2%AD%90)
- [awesome-open-source-solvers](https://github.com/shvyac/awesome-open-source-solvers) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-open-source-solvers?style=flat&label=%E2%AD%90)
- [awesome-osint-ai](https://github.com/shvyac/awesome-osint-ai) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-osint-ai?style=flat&label=%E2%AD%90)
- [awesome-redmine-ai](https://github.com/shvyac/awesome-redmine-ai) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-redmine-ai?style=flat&label=%E2%AD%90)
- [awesome-requirements-system-ai](https://github.com/shvyac/awesome-requirements-system-ai) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-requirements-system-ai?style=flat&label=%E2%AD%90)
- [awesome-trading-stock](https://github.com/shvyac/awesome-trading-stock) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-trading-stock?style=flat&label=%E2%AD%90)
