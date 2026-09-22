# 機械工学のためのAwesome AIツール

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

**機械設計ワークフロー向けのAIコパイロットとプラットフォーム** — 商用CADアシスタント、ジェネレーティブデザイン、CAEサロゲート、DFMレビュー、V&Vまで。エージェント呼び出し可能なOSSだけに限定しません。

**対象範囲:** 機械エンジニア向けに、**CAD → CAE → レビュー → V&V** にわたる商用＋オープンツール。

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

---

## CADコパイロット & Text-to-CAD

MCAD内（または隣接）でモデリングを加速する自然言語アシスタントとText-to-CAD。

- [SOLIDWORKS AI Companions (AURA & LEO)](https://www.solidworks.com/product/solidworks-design/ai-companions) — アプリ内コンパニオン。AURAは社内/Webナレッジ、LEOは会話型の設計支援。Tags: `Commercial`
- [Creo AI Assistant](https://support.ptc.com/help/creo/creo_ai/usascii/ai_assistant/overview.html) — Creo内でのドキュメント参照、モデル文脈Q&A、CAD作業支援。Tags: `Commercial`
- [Autodesk Assistant in Inventor](https://help.autodesk.com/view/INVNTOR/2027/ENU/?guid=ABOUT-AUTODESK-ASSISTANT-INVENTOR) — Inventor向け自然言語ヘルプ、モデル照会、タスク自動化。Tags: `Commercial`
- [MecAgent](https://mecagent.com/) — SOLIDWORKS & Inventor向けコパイロット。Text-to-マクロ、図面自動化、工学Q&A、実験的Text-to-STEP/STL。Tags: `Commercial`
- [Zoo Design Studio](https://zoo.dev/) — 会話型Text-to-CADを備えたAIネイティブCAD（編集可能なB-rep / KCL）。Tags: `Commercial`
- [Leo AI](https://www.getleo.ai/) — 仕様/スケッチからのアセンブリ生成と、ボルト内の形状ベース部品検索。Tags: `Commercial`
- [CATIA / 3DEXPERIENCE](https://www.3ds.com/products/catia) — ジオメトリ支援とプラットフォーム知識ワークフロー向けDassault AI。Tags: `Commercial`
- [Siemens NX AI](https://www.siemens.com/en-us/products/designcenter/cad-software/ai/) — NXのコマンド予測、性能予測、ジェネレーティブ/トポロジー。Tags: `Commercial`

## ジェネレーティブデザイン & トポロジー最適化

荷重・材料・製法制約に基づく形状生成と軽量化。

- [Autodesk Fusion Generative Design](https://www.autodesk.com/products/fusion-360/) — Fusion内の多目的ジェネレーティブデザイン（製造制約付き代替案）。Tags: `Commercial`
- [PTC Creo Generative Design](https://www.ptc.com/en/technologies/cad/generative-design) — Creo GTO / GDXによる制約駆動のコンセプト探索。Tags: `Commercial`
- [nTop](https://www.ntop.com/) — ラティス、トポロジーソリッド、共形流路、AM向け形状のフィールド駆動/陰関数設計。Tags: `Commercial`
- [Simcenter Inspire](https://www.siemens.com/en-us/products/simcenter/mechanical-simulation/inspire/) — 設計者向けトポロジー最適化と構造コンセプト検討。Tags: `Commercial`
- [Ansys GeomAI](https://www.ansys.com/products/ai/geomai) — 参照形状から学習してコンセプト探索。SimAI/ソルバーと連携。Tags: `Commercial`
- ネイティブCADトポロジー機能 — Fusion、Creo、SOLIDWORKS Simulation、NX Topology Optimizationなどの組み込み軽量化。Tags: `Commercial`

## シミュレーション、CAE & サロゲートAI

セットアップ高速化、リアルタイムWhat-if、過去CAEデータからの場予測。

- [Ansys SimAI](https://www.ansys.com/products/ai/simai) — 既存シミュレーション結果で学習し、新設計の3D場を予測。Tags: `Commercial`
- [Ansys Discovery](https://www.ansys.com/products/3d-design/ansys-discovery) — GPU上のリアルタイム構造/熱/流体探索。本格ソルバーへの引き継ぎも。Tags: `Commercial`
- [Simcenter PhysicsAI](https://www.siemens.com/en-us/products/simcenter/engineering-data-science-ai/physicsai/) — CAEデータ上の幾何深層学習による高速物理予測。Tags: `Commercial`
- [Neural Concept](https://www.neuralconcept.com/) — 形状ベースAIによるリアルタイムマルチフィジックス予測と設計空間探索。Tags: `Commercial`
- [SimScale](https://www.simscale.com/) — AI支援セットアップ付きクラウドFEA/CFD/熱解析。Tags: `Commercial`

## Physics-ML、PINNs & オープンフレームワーク

学習ループを自前で回すときのオープンなPINNs / ニューラル演算子 / ハイブリッドPhysics-ML。

- [NVIDIA PhysicsNeMo](https://developer.nvidia.com/physicsnemo) — PINNs、ニューラル演算子、GNN、ハイブリッドPhysics-ML向けPyTorchフレームワーク（[GitHub](https://github.com/NVIDIA/physicsnemo)）。Tags: `OSS`
- [DeepXDE](https://deepxde.readthedocs.io/) — PINNs / PDE向け深層学習の定番ライブラリ。教育・研究の入口に適する（[GitHub](https://github.com/lululxvi/deepxde)）。Tags: `OSS`

## CAD検索、PDM & ナレッジ

新規形状を作る前に、検証済み部品と社内知を再利用。

- [SOLIDWORKS AURA](https://www.solidworks.com/product/solidworks-design/ai-companions) — 設計環境内で社内ナレッジ、3DSwym、ドキュメントへ接続。Tags: `Commercial`
- 形状ベースの類似部品検索は [Leo AI](#cadコパイロット--text-to-cad) も参照。

## DFM、GD&T & デザインレビュー

図面/モデルレビュー、変更検出、製造性チェックの自動化。

- [bananaz](https://www.bananaz.ai/) — CAD/図面差分、DFM、GD&T/公差レビュー、赤入れ向けAIエージェント。Tags: `Commercial`
- [CoLab AutoReview](https://www.colabsoftware.com/product/autoreview) — モデルと図面のAIレビュー（GD&T、完全性、規格、DFM）と追跡可能なマークアップ。Tags: `Commercial`

## V&V（検証・妥当性確認）

物理試作を減らし、シミュレーション根拠を追跡可能にするMLとSPDM。

- [Monolith AI](https://www.monolithai.com/) — 仮想テスト向けML。過去の試験/シミュレーションから結果を予測し試作ループを縮小。Tags: `Commercial`
- [Ansys Minerva](https://www.ansys.com/products/connect/ansys-minerva) — 追跡・監査可能なシミュレーションV&V向けSPDM。Tags: `Commercial`
- [Siemens Simcenter Testlab](https://www.siemens.com/en-us/products/simcenter/physical-testing/testlab/) — 物理試験/NVH解析と試験↔シミュレーション相関。Tags: `Commercial`
- [COMSOL Model Manager](https://www.comsol.com/model-manager) — V&Vライフサイクル全体でマルチフィジックスモデルを版管理・検証。Tags: `Commercial`

## MCP & エージェントツール

CAD/CAEアプリと対話するエージェント向けの短いポインタ。本リストは**機械設計ワークフロー優先**（商用含む）。OSSのエージェント呼び出し可能性ランキングは [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) を参照。

- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) — CAD/デザイン向けMCPコネクタ等のキュレーション（Fusion MCP、Blender Lab MCP、SketchUpなど）。Tags: `OSS`
- [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) — エージェント呼び出し可能なOSS CAE/CADスタック（MCP / Python / CLI）とレディネス評価。Tags: `OSS`

## 関連Awesomeリスト

- [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) — AI呼び出し可能なCAE/CADツールとエージェントレディネス。Tags: `OSS`
- [awesome-cad-cae](https://github.com/shvyac/awesome-cad-cae) — CAD/CAEアプリ、カーネル、FEA/CFD、トポロジー最適化。Tags: `OSS`
- [awesome-open-source-solvers](https://github.com/shvyac/awesome-open-source-solvers) — オープンなFEM/CFD/MBD/粒子ソルバーと科学計算スタック。Tags: `OSS`
- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) — ハードウェアエンジニアリング向けAI（CAD、シミュレーション、製造）。Tags: `OSS`
- [awesome-mechanical-engineering](https://github.com/awesomelistsio/awesome-mechanical-engineering) — より広い機械工学ツール、プラットフォーム、学習リソース。Tags: `OSS`

## 自動車V&V（深掘り）

車両HIL / ECU V&V向けの短い任意セクション。自動車の制御・試験でなければスキップして問題ありません。

### HIL & テストツール

- [dSPACE SCALEXIO / ASM](https://www.dspace.com/) — HILシステムと車両/ECUシミュレーションモデル。Tags: `Commercial`
- [Vector CANoe](https://www.vector.com/int/en/products/products-a-z/software/canoe/) — ECU・ネットワークの開発、テスト、解析。Tags: `Commercial`
- [NI VeriStand](https://www.ni.com/en/shop/veristand.html) — リアルタイムHIL、モデル検証、迅速な制御プロトタイピング。Tags: `Commercial`
- [MathWorks Simulink Test](https://www.mathworks.com/products/simulink-test.html) — 要求トレーサビリティとモデル検証の自動化。Tags: `Commercial`
- [ETAS LABCAR](https://www.etas.com/en/products/labcar.php) — 実運用条件に近いECU妥当性確認向けHIL。Tags: `Commercial`
- [ASAM ODS](https://www.asam.net/standards/detail/ods/) — 計測・シミュレーション・妥当性確認データの交換標準。Tags: `Commercial`

ODSエコシステムへのポインタ（網羅カタログではありません）: [Peak ODS Server](https://www.peak-solution.com/)、[openMDM](https://openmdm.org/)、[AVL CONCERTO](https://www.avl.com/)。

### オープンソースMBSE / シナリオ（少数）

- [Eclipse Capella](https://github.com/eclipse-capella/capella) — システムレベル間のアーキテクチャ分解向けArcadia MBSE。Tags: `OSS`
- [CARLA](https://github.com/carla-simulator/carla) + [esmini / OpenSCENARIO](https://github.com/esmini/esmini) — シナリオレベルV&V向けオープン運転シミュレータとシナリオ標準。Tags: `OSS`
- [openMDM](https://openmdm.org/) — ASAM ODSベースの試験データ管理向けEclipseコンポーネント。Tags: `OSS`

## コントリビューション

コントリビューション歓迎です。ツール追加、リンク修正、カテゴリ提案はPRを開いてください。

**公式/ドキュメントの耐久性のあるURL**、一文の短い説明、実出荷ツールを優先。各エントリに `Commercial` または `OSS` を付けてください。ENとJAのREADMEは同期を保ってください。

## ライセンス

[LICENSE](LICENSE) を参照してください。
