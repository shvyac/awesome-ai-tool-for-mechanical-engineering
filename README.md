# Awesome AI Tools for Mechanical Engineering

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

**AI copilots and platforms for the mechanical workflow** — commercial CAD assistants, generative design, CAE surrogates, DFM review, and V&V — not only agent-callable OSS.

**Scope:** commercial + open tools across **CAD → CAE → review → V&V** for mechanical engineers.

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

---

## CAD Copilots & Text-to-CAD

Natural-language assistants and text-to-CAD that accelerate modeling inside (or next to) MCAD.

- [SOLIDWORKS AI Companions (AURA & LEO)](https://www.solidworks.com/product/solidworks-design/ai-companions) — In-app companions: AURA for enterprise/web knowledge, LEO for conversational design help. Tags: `Commercial`
- [Creo AI Assistant](https://support.ptc.com/help/creo/creo_ai/usascii/ai_assistant/overview.html) — In-Creo docs, model-context Q&A, and assisted CAD tasks. Tags: `Commercial`
- [Autodesk Assistant in Inventor](https://help.autodesk.com/view/INVNTOR/2027/ENU/?guid=ABOUT-AUTODESK-ASSISTANT-INVENTOR) — Natural-language help, model queries, and task automation in Inventor. Tags: `Commercial`
- [MecAgent](https://mecagent.com/) — SOLIDWORKS & Inventor copilot: text-to-macros, drawing automation, engineering Q&A, experimental text-to-STEP/STL. Tags: `Commercial`
- [Zoo Design Studio](https://zoo.dev/) — AI-native CAD with conversational text-to-CAD (editable B-rep / KCL). Tags: `Commercial`
- [Leo AI](https://www.getleo.ai/) — Spec/sketch → assemblies plus shape-based part search across your vault. Tags: `Commercial`
- [CATIA / 3DEXPERIENCE](https://www.3ds.com/products/catia) — Dassault AI for geometry assistance and platform knowledge workflows. Tags: `Commercial`
- [Siemens NX AI](https://www.siemens.com/en-us/products/designcenter/cad-software/ai/) — Command prediction, performance predictors, and generative/topology workflows in NX. Tags: `Commercial`

## Generative Design & Topology Optimization

Constraint-driven geometry and lightweighting (loads, materials, manufacturing methods).

- [Autodesk Fusion Generative Design](https://www.autodesk.com/products/fusion-360/) — Multi-objective generative design in Fusion with manufacturing-aware alternatives. Tags: `Commercial`
- [PTC Creo Generative Design](https://www.ptc.com/en/technologies/cad/generative-design) — Creo GTO / GDX for constraint-driven concept exploration. Tags: `Commercial`
- [nTop](https://www.ntop.com/) — Field-driven / implicit design for lattices, topology solids, conformal channels, AM-ready geometry. Tags: `Commercial`
- [Simcenter Inspire](https://www.siemens.com/en-us/products/simcenter/mechanical-simulation/inspire/) — Designer-facing topology optimization and structural concepting. Tags: `Commercial`
- [Ansys GeomAI](https://www.ansys.com/products/ai/geomai) — Learns from reference geometries to explore concepts; pairs with SimAI / solvers. Tags: `Commercial`
- Native CAD topology studies — Built-in lightweighting in Fusion, Creo, SOLIDWORKS Simulation, and NX Topology Optimization. Tags: `Commercial`

## Simulation, CAE & Surrogate AI

Faster setup, real-time what-if exploration, or field prediction from past CAE data.

- [Ansys SimAI](https://www.ansys.com/products/ai/simai) — Train on legacy simulation results to predict 3D fields for new designs. Tags: `Commercial`
- [Ansys Discovery](https://www.ansys.com/products/3d-design/ansys-discovery) — Real-time structural / thermal / fluid exploration on GPU, with handoff to flagship solvers. Tags: `Commercial`
- [Simcenter PhysicsAI](https://www.siemens.com/en-us/products/simcenter/engineering-data-science-ai/physicsai/) — Geometric deep learning on CAE data for fast physics across meshes/topologies. Tags: `Commercial`
- [Neural Concept](https://www.neuralconcept.com/) — Geometry-aware AI for real-time multiphysics prediction and design-space exploration. Tags: `Commercial`
- [SimScale](https://www.simscale.com/) — Cloud FEA/CFD/thermal with AI-assisted setup and collaboration. Tags: `Commercial`

## Physics-ML, PINNs & Open Frameworks

Open stacks when you own the training loop (PINNs, neural operators, hybrid Physics-ML).

- [NVIDIA PhysicsNeMo](https://developer.nvidia.com/physicsnemo) — PyTorch framework for PINNs, neural operators, GNNs, and hybrid Physics-ML ([GitHub](https://github.com/NVIDIA/physicsnemo)). Tags: `OSS`
- [DeepXDE](https://deepxde.readthedocs.io/) — Popular PINNs / deep-learning-for-PDEs library; strong teaching entry point ([GitHub](https://github.com/lululxvi/deepxde)). Tags: `OSS`

## CAD Search, PDM & Knowledge

Reuse validated parts and tribal knowledge instead of reinventing geometry.

- [SOLIDWORKS AURA](https://www.solidworks.com/product/solidworks-design/ai-companions) — Connects designers to company knowledge, 3DSwym, and docs inside the design environment. Tags: `Commercial`
- See also [Leo AI](#cad-copilots--text-to-cad) for shape-based similar-part search in vaults/PDM.

## DFM, GD&T & Design Review

Automated drawing/model review, change detection, and manufacturability checks.

- [bananaz](https://www.bananaz.ai/) — AI agents for CAD/drawing diffs, DFM, GD&T/tolerance review, and redlines. Tags: `Commercial`
- [CoLab AutoReview](https://www.colabsoftware.com/product/autoreview) — AI reviews on models and drawings (GD&T, completeness, standards, DFM) with tracked markups. Tags: `Commercial`

## V&V (Verification & Validation)

ML and SPDM that cut physical prototypes and keep simulation evidence traceable.

- [Monolith AI](https://www.monolithai.com/) — ML for virtual testing: predict outcomes from past tests/sims and shrink prototype loops. Tags: `Commercial`
- [Ansys Minerva](https://www.ansys.com/products/connect/ansys-minerva) — SPDM for traceable, auditable simulation V&V workflows. Tags: `Commercial`
- [Siemens Simcenter Testlab](https://www.siemens.com/en-us/products/simcenter/physical-testing/testlab/) — Physical testing / NVH analytics with test↔simulation correlation. Tags: `Commercial`
- [COMSOL Model Manager](https://www.comsol.com/model-manager) — Version-control and verify multiphysics models across the V&V lifecycle. Tags: `Commercial`

## MCP & Agent Tooling

Brief pointers for agents that talk to CAD/CAE apps. This list stays **ME-workflow first** (including commercial tools); for OSS agent-callability rankings, see [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae).

- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) — Curated MCP connectors and AI tooling for CAD/design (e.g. Fusion MCP, Blender Lab MCP, SketchUp). Tags: `OSS`
- [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) — Agent-callable OSS CAE/CAD stack (MCP / Python / CLI), with readiness ranking. Tags: `OSS`

## Related Awesome Lists

- [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) — AI-callable CAE/CAD tooling and agent readiness. Tags: `OSS`
- [awesome-cad-cae](https://github.com/shvyac/awesome-cad-cae) — CAD/CAE apps, kernels, FEA/CFD, topology optimization. Tags: `OSS`
- [awesome-open-source-solvers](https://github.com/shvyac/awesome-open-source-solvers) — Open FEM/CFD/MBD/particle solvers and scientific stacks. Tags: `OSS`
- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) — Broader hardware-engineering AI (CAD, sim, manufacturing). Tags: `OSS`
- [awesome-mechanical-engineering](https://github.com/awesomelistsio/awesome-mechanical-engineering) — Broader ME tools, platforms, and learning resources. Tags: `OSS`

## Automotive V&V (deep-dive)

Optional short list for vehicle HIL / ECU V&V. Skip unless you work automotive control & test.

### HIL & test tooling

- [dSPACE SCALEXIO / ASM](https://www.dspace.com/) — HIL systems and vehicle/ECU simulation models. Tags: `Commercial`
- [Vector CANoe](https://www.vector.com/int/en/products/products-a-z/software/canoe/) — ECU & network development, testing, and analysis. Tags: `Commercial`
- [NI VeriStand](https://www.ni.com/en/shop/veristand.html) — Real-time HIL, model validation, and rapid control prototyping. Tags: `Commercial`
- [MathWorks Simulink Test](https://www.mathworks.com/products/simulink-test.html) — Requirements traceability and automated model verification. Tags: `Commercial`
- [ETAS LABCAR](https://www.etas.com/en/products/labcar.php) — HIL environment for ECU validation under realistic conditions. Tags: `Commercial`
- [ASAM ODS](https://www.asam.net/standards/detail/ods/) — Standard for exchanging measurement, simulation, and validation data. Tags: `Commercial`

Pointers into the ODS ecosystem (not a full vendor catalog): [Peak ODS Server](https://www.peak-solution.com/), [openMDM](https://openmdm.org/), [AVL CONCERTO](https://www.avl.com/).

### Open-source MBSE / scenario (few)

- [Eclipse Capella](https://github.com/eclipse-capella/capella) — Arcadia MBSE for architecture decomposition across system levels. Tags: `OSS`
- [CARLA](https://github.com/carla-simulator/carla) + [esmini / OpenSCENARIO](https://github.com/esmini/esmini) — Open driving simulator and scenario standards for scenario-level V&V. Tags: `OSS`
- [openMDM](https://openmdm.org/) — Eclipse components for ASAM ODS–based test data management. Tags: `OSS`

## Contributing

Contributions welcome — open a PR to add a tool, fix a link, or suggest a category.

Prefer **durable official / docs URLs**, one crisp sentence, and tools that are shipping. Tag each entry `Commercial` or `OSS`. Keep EN and JA READMEs in sync.

## License

See [LICENSE](LICENSE).
