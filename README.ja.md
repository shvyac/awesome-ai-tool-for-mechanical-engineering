# 機械工学のためのAwesome AIツール

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

**機械設計ワークフロー向けのAIコパイロットとプラットフォーム** — 商用CADアシスタント、ジェネレーティブデザイン、CAEサロゲート、DFMレビュー、V&Vまで。エージェント呼び出し可能なOSSだけに限定しません。

**対象範囲:** 機械エンジニア向けに、**CAD → CAE → レビュー → V&V** にわたる商用＋オープンツール。

⭐ バッジは GitHub のスター数をリアルタイム表示します(shields.io)。リリースバッジは最新リリースの版数と日付を表示します。

[English](README.md)

## まずはここから

| やりたいこと | 向かう先 |
| --- | --- |
| CADでモデリングを速くしたい | [CADコパイロット & Text-to-CAD](#cadコパイロット--text-to-cad) |
| 形状探索・軽量化 | [ジェネレーティブデザイン & トポロジー最適化](#ジェネレーティブデザイン--トポロジー最適化) |
| What-if物理を速く回したい | [シミュレーション、CAE & サロゲートAI](#シミュレーションcae--サロゲートai) |
| 自前でPhysics-MLを学習したい | [Physics-ML、PINNs & オープンフレームワーク](#physics-mlpinns--オープンフレームワーク) |
| 部品・ナレッジを再利用したい | [CAD検索、PDM & ナレッジ](#cad検索pdm--ナレッジ) |
| 図面・DFMをチェックしたい | [DFM、GD&T & デザインレビュー](#dfmgdt--デザインレビュー) |
| 試験とシミュレーションを追跡したい | [V&V（検証・妥当性確認）](#vv検証妥当性確認) |
| エージェント / MCPコネクタ | [MCP & エージェントツール](#mcp--エージェントツール) |

## 目次

- [CADコパイロット & Text-to-CAD](#cadコパイロット--text-to-cad)
- [ジェネレーティブデザイン & トポロジー最適化](#ジェネレーティブデザイン--トポロジー最適化)
- [シミュレーション、CAE & サロゲートAI](#シミュレーションcae--サロゲートai)
- [Physics-ML、PINNs & オープンフレームワーク](#physics-mlpinns--オープンフレームワーク)
- [CAD検索、PDM & ナレッジ](#cad検索pdm--ナレッジ)
- [DFM、GD&T & デザインレビュー](#dfmgdt--デザインレビュー)
- [V&V（検証・妥当性確認）](#vv検証妥当性確認)
- [MCP & エージェントツール](#mcp--エージェントツール)
- [関連Awesomeリスト](#関連awesomeリスト)
- [自動車V&V（深掘り）](#自動車vv深掘り)
- [コントリビューション](#コントリビューション)
- [ライセンス](#ライセンス)
- [shvyac の awesome リスト](#shvyac-の-awesome-リスト)

---

## CADコパイロット & Text-to-CAD

MCAD内（または隣接）でモデリングを加速する自然言語アシスタントとText-to-CAD。

- [SOLIDWORKS AI Virtual Companions (AURA, LEO & MARIE)](https://www.solidworks.com/product/solidworks-design/ai-virtual-companions) — アプリ内コンパニオン。AURAは社内/Webナレッジ、LEOは会話型の設計支援、MARIEは材料選定支援。Tags: `Commercial`
- [Creo AI Assistant](https://support.ptc.com/help/creo/creo_ai/usascii/ai_assistant/overview.html) — Creo内のエージェント。Creo Advise（無料、ドキュメント参照・モデル文脈Q&A）とCreo Assist（CAD作業支援、Advanced AIライセンス）。Tags: `Commercial`
- [Autodesk Assistant in Inventor](https://www.autodesk.com/blogs/design-and-manufacturing/meet-autodesk-assistant-in-inventor-2027/) — Inventor向け自然言語ヘルプ、モデル照会、タスク自動化（Inventor 2027以降）。Tags: `Commercial`
- [MecAgent](https://mecagent.com/) — SOLIDWORKS & Inventor向けコパイロットと、SOLIDWORKS内で動くV2エージェント。Text/Image-to-CAD、図面からのCAD化、アセンブリ、BOM、マクロ、図面作成（Onshape版も予定）。Tags: `Commercial`
- [Zoo Design Studio](https://zoo.dev/) — Zookeeperエージェントによる会話型Text-to-CADを備えたAIネイティブCAD（編集可能なB-rep / KCL）。Tags: `Commercial`
- [Leo AI](https://www.getleo.ai/) — 仕様/スケッチからのアセンブリ生成と、ボルト内の形状ベース部品検索。Tags: `Commercial`
- [Adam](https://adam.new/) — ハードウェアチーム向けAI CADコパイロット（YC）。SlackやメールでOnshape、Fusion、SOLIDWORKSの作業を依頼すると、ブランチ上のモデル編集、BOM、図面、サプライヤー見積を返す。Tags: `Commercial`
- [CATIA / 3DEXPERIENCE](https://www.3ds.com/products/catia) — ジオメトリ支援とプラットフォーム知識ワークフロー向けDassault AI。Tags: `Commercial`
- [Siemens NX AI](https://www.siemens.com/en-us/products/designcenter/cad-software/ai/) — NXのコマンド予測、性能予測、ジェネレーティブ/トポロジー（現在はSiemens Designcenterの一部）。Tags: `Commercial`

## ジェネレーティブデザイン & トポロジー最適化

荷重・材料・製法制約に基づく形状生成と軽量化。

- [Autodesk Fusion Generative Design](https://www.autodesk.com/products/fusion-360/) — Autodesk Fusion（旧Fusion 360）内の多目的ジェネレーティブデザイン（製造制約付き代替案）。Tags: `Commercial`
- [PTC Creo Generative Design](https://www.ptc.com/en/technologies/cad/generative-design) — Creo GTO / GDXによる制約駆動のコンセプト探索。Tags: `Commercial`
- [nTop](https://www.ntop.com/) — ラティス、トポロジーソリッド、共形流路、AM向け形状のフィールド駆動/陰関数設計。Tags: `Commercial`
- [Simcenter Inspire](https://www.siemens.com/en-us/products/simcenter/mechanical-simulation/inspire/) — 設計者向けトポロジー最適化と構造コンセプト検討（旧Altair Inspire、現在はSimcenterファミリー）。Tags: `Commercial`
- [Ansys GeomAI](https://ansys.synopsys.com/products/ai/geomai) — 参照形状から学習してコンセプト探索。SimAI/ソルバーと連携（AnsysはSynopsys傘下）。Tags: `Commercial`
- ネイティブCADトポロジー機能 — Fusion、Creo、SOLIDWORKS Simulation、NX Topology Optimizationなどの組み込み軽量化。Tags: `Commercial`

## シミュレーション、CAE & サロゲートAI

セットアップ高速化、リアルタイムWhat-if、過去CAEデータからの場予測。

- [AgentFEM](https://haoming-luo.github.io/agentfem/) — ローカルのFEniCSx実行環境で、AIエージェントによる編集可能なPythonモデルの作成、計算前の設定確認、有限要素計算、結果の確認を支援（[GitHub](https://github.com/haoming-luo/agentfem)）。Tags: `OSS`
- [Ansys SimAI](https://www.ansys.com/products/ai/simai) — 既存シミュレーション結果で学習し、新設計の3D場を予測。SimAI Pro / SimAI Premiumの2プラン。Tags: `Commercial`
- [Ansys Discovery](https://ansys.synopsys.com/products/3d-design/ansys-discovery) — GPU上のリアルタイム構造/熱/流体探索。本格ソルバーへの引き継ぎも（AnsysはSynopsys傘下）。Tags: `Commercial`
- [Simcenter PhysicsAI](https://www.siemens.com/en-us/products/simcenter/engineering-data-science-ai/physicsai/) — CAEデータ上の幾何深層学習による高速物理予測。Tags: `Commercial`
- [Neural Concept](https://www.neuralconcept.com/) — 形状ベースAIによるリアルタイムマルチフィジックス予測と設計空間探索。Tags: `Commercial`
- [PhysicsX](https://www.physicsx.ai/) — シミュレーション、Physics AI、データを統合したAIネイティブなエンジニアリング基盤。設計・製造・運用をカバー。Tags: `Commercial`
- [Luminary](https://luminary.ai/) — 「Large Physics Models」を学習・展開するPhysics AIプラットフォーム（旧Luminary Cloud）。流れ・構造・熱を1秒未満で予測。Tags: `Commercial`
- [SimScale](https://www.simscale.com/) — AI支援セットアップ付きクラウドFEA/CFD/熱解析。Tags: `Commercial`

## Physics-ML、PINNs & オープンフレームワーク

学習ループを自前で回すときのオープンなPINNs / ニューラル演算子 / ハイブリッドPhysics-ML。

- [NVIDIA PhysicsNeMo](https://developer.nvidia.com/physicsnemo) ![GitHub stars](https://img.shields.io/github/stars/NVIDIA/physicsnemo?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/NVIDIA/physicsnemo?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/NVIDIA/physicsnemo?style=flat&label=released) — PINNs、ニューラル演算子、GNN、ハイブリッドPhysics-ML向けPyTorchフレームワーク（[GitHub](https://github.com/NVIDIA/physicsnemo)）。Tags: `OSS`
- [DeepXDE](https://deepxde.readthedocs.io/) ![GitHub stars](https://img.shields.io/github/stars/lululxvi/deepxde?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/lululxvi/deepxde?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/lululxvi/deepxde?style=flat&label=released) — PINNs / PDE向け深層学習の定番ライブラリ。教育・研究の入口に適する（[GitHub](https://github.com/lululxvi/deepxde)）。Tags: `OSS`

## CAD検索、PDM & ナレッジ

新規形状を作る前に、検証済み部品と社内知を再利用。

- [SOLIDWORKS AURA](https://www.solidworks.com/product/solidworks-design/ai-virtual-companions) — 設計環境内で社内ナレッジ、3DSwym、ドキュメントへ接続。Tags: `Commercial`
- 形状ベースの類似部品検索は [Leo AI](#cadコパイロット--text-to-cad) も参照。

## DFM、GD&T & デザインレビュー

図面/モデルレビュー、変更検出、製造性チェックの自動化。

- [bananaz](https://www.bananaz.ai/) — CAD/図面差分、DFM、GD&T/公差レビュー、赤入れ向けAIエージェント。Tags: `Commercial`
- [CoLab AutoReview](https://www.colabsoftware.com/product/autoreview) — モデルと図面のAIレビュー（GD&T、完全性、規格、DFM）と追跡可能なマークアップ。初期顧客へ順次提供中（ウェイトリスト）。Tags: `Commercial`

## V&V（検証・妥当性確認）

物理試作を減らし、シミュレーション根拠を追跡可能にするMLとSPDM。

- [Monolith](https://www.monolithai.com/) — 仮想テスト向けML。過去の試験/シミュレーションから結果を予測し試作ループを縮小（現在はCoreWeave傘下）。Tags: `Commercial`
- [Ansys Minerva](https://ansys.synopsys.com/products/connect/ansys-minerva) — 追跡・監査可能なシミュレーションV&V向けSPDM（Arasベース）。Tags: `Commercial`
- [Siemens Simcenter Testlab](https://www.siemens.com/en-us/products/simcenter/physical-testing/testlab/) — 物理試験/NVH解析と試験↔シミュレーション相関。Tags: `Commercial`
- [COMSOL Model Manager](https://www.comsol.com/comsol-multiphysics/model-manager) — V&Vライフサイクル全体でマルチフィジックスモデルを版管理・検証。Tags: `Commercial`

## MCP & エージェントツール

CAD/CAEアプリと対話するエージェント向けの短いポインタ。本リストは**機械設計ワークフロー優先**（商用含む）。OSSのエージェント呼び出し可能性ランキングは [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) を参照。

- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) ![GitHub stars](https://img.shields.io/github/stars/010zx00x1/Awesome-Physical-Engineering-AI?style=flat&label=%E2%AD%90) — CAD/デザイン向けMCPコネクタ等のキュレーション（Fusion MCP、Blender Lab MCP、SketchUpなど）。Tags: `OSS`
- [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) ![GitHub stars](https://img.shields.io/github/stars/kimimgo/awesome-ai-cae?style=flat&label=%E2%AD%90) — エージェント呼び出し可能なOSS CAE/CADスタック（MCP / Python / CLI）とレディネス評価。Tags: `OSS`
- [Autodesk Fusion MCP](https://www.autodesk.com/products/fusion-360/blog/introducing-the-fusion-mcp-opening-fusion-to-ai-powered-workflows/) — AIクライアントからFusion内で設計の作成・編集を行う公式MCPサーバー（デスクトップ）と、プロジェクトデータを扱うFusion Data MCP Server。Tags: `Commercial`
- [Onshape FeatureScript MCP Server](https://www.onshape.com/en/features/onshape-labs) — Onshape Labs（PTC）のアーリーアクセス。AIクライアントがFeatureScriptを記述・実行・修正し、再利用可能なパラメトリックなカスタムフィーチャーを作成。Tags: `Commercial`
- [text-to-cad](https://github.com/earthtojake/text-to-cad) ![GitHub stars](https://img.shields.io/github/stars/earthtojake/text-to-cad?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/earthtojake/text-to-cad?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/earthtojake/text-to-cad?style=flat&label=released) — AIコーディングエージェントにCAD機能（STEP/STL出力）を与えるオープンソースのツールキット。2026年10月にGitHubでトレンド入り。Tags: `OSS`

## 関連Awesomeリスト

- [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) ![GitHub stars](https://img.shields.io/github/stars/kimimgo/awesome-ai-cae?style=flat&label=%E2%AD%90) — AI呼び出し可能なCAE/CADツールとエージェントレディネス。Tags: `OSS`
- [awesome-cad-cae](https://github.com/shvyac/awesome-cad-cae) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-cad-cae?style=flat&label=%E2%AD%90) — CAD/CAEアプリ、カーネル、FEA/CFD、トポロジー最適化。Tags: `OSS`
- [awesome-open-source-solvers](https://github.com/shvyac/awesome-open-source-solvers) ![GitHub stars](https://img.shields.io/github/stars/shvyac/awesome-open-source-solvers?style=flat&label=%E2%AD%90) — オープンなFEM/CFD/MBD/粒子ソルバーと科学計算スタック。Tags: `OSS`
- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) ![GitHub stars](https://img.shields.io/github/stars/010zx00x1/Awesome-Physical-Engineering-AI?style=flat&label=%E2%AD%90) — ハードウェアエンジニアリング向けAI（CAD、シミュレーション、製造）。Tags: `OSS`
- [awesome-mechanical-engineering](https://github.com/brandonhimpfen/awesome-mechanical-engineering) ![GitHub stars](https://img.shields.io/github/stars/brandonhimpfen/awesome-mechanical-engineering?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/brandonhimpfen/awesome-mechanical-engineering?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/brandonhimpfen/awesome-mechanical-engineering?style=flat&label=released) — より広い機械工学ツール、プラットフォーム、学習リソース。Tags: `OSS`

## 自動車V&V（深掘り）

車両HIL / ECU V&V向けの短い任意セクション。自動車の制御・試験でなければスキップして問題ありません。

### HIL & テストツール

- [dSPACE SCALEXIO / ASM](https://www.dspace.com/) — HILシステムと車両/ECUシミュレーションモデル。Tags: `Commercial`
- [Vector CANoe](https://www.vector.com/en/product/canoe/) — ECU・ネットワークの開発、テスト、解析（SIL & HIL）。Tags: `Commercial`
- [NI VeriStand](https://www.ni.com/en-us/shop/product/veristand.html) — リアルタイムHIL、モデル検証、迅速な制御プロトタイピング（NIは現在Emerson傘下）。Tags: `Commercial`
- [MathWorks Simulink Test](https://www.mathworks.com/products/simulink-test.html) — 要求トレーサビリティとモデル検証の自動化。Tags: `Commercial`
- [ETAS LABCAR](https://www.etas.com/ww/en/products-services/) — 実運用条件に近いECU妥当性確認向けHIL。Tags: `Commercial`
- [ASAM ODS](https://www.asam.net/standards/detail/ods/) — 計測・シミュレーション・妥当性確認データの交換標準。Tags: `Commercial`

ODSエコシステムへのポインタ（網羅カタログではありません）: [Peak ODS Server](https://www.peak-solution.com/)、[openMDM](https://openmdm.org/)、[AVL CONCERTO](https://www.avl.com/)。

### オープンソースMBSE / シナリオ（少数）

- [Eclipse Capella](https://github.com/eclipse-capella/capella) ![GitHub stars](https://img.shields.io/github/stars/eclipse-capella/capella?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/eclipse-capella/capella?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/eclipse-capella/capella?style=flat&label=released) — システムレベル間のアーキテクチャ分解向けArcadia MBSE。Tags: `OSS`
- [CARLA](https://github.com/carla-simulator/carla) ![GitHub stars](https://img.shields.io/github/stars/carla-simulator/carla?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/carla-simulator/carla?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/carla-simulator/carla?style=flat&label=released) + [esmini / OpenSCENARIO](https://github.com/esmini/esmini) ![GitHub stars](https://img.shields.io/github/stars/esmini/esmini?style=flat&label=%E2%AD%90) ![GitHub release](https://img.shields.io/github/v/release/esmini/esmini?style=flat&label=release) ![GitHub release date](https://img.shields.io/github/release-date/esmini/esmini?style=flat&label=released) — シナリオレベルV&V向けオープン運転シミュレータとシナリオ標準。Tags: `OSS`
- [openMDM](https://openmdm.org/) — ASAM ODSベースの試験データ管理向けEclipseコンポーネント（Eclipseワーキンググループは活動終了）。Tags: `OSS`

## コントリビューション

コントリビューション歓迎です。ツール追加、リンク修正、カテゴリ提案はPRを開いてください。

**公式/ドキュメントの耐久性のあるURL**、一文の短い説明、実出荷ツールを優先。各エントリに `Commercial` または `OSS` を付けてください。ENとJAのREADMEは同期を保ってください。

## ライセンス

[LICENSE](LICENSE) を参照してください。

## shvyac の awesome リスト

[shvyac](https://github.com/shvyac) が管理しているキュレーションリストの一覧:

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
