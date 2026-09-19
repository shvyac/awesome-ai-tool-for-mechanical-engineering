# 機械工学のためのAwesome AIツール

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

機械工学向けのAI搭載ツール、コパイロット、プラットフォームのキュレーションリストです。CAD、CAE/シミュレーション、ジェネレーティブデザイン、トポロジー最適化、デザインレビュー、Physics-MLサロゲート、製造考慮ワークフロー、V&Vをカバーします。

[English](README.md)

## 目次

- [CADコパイロット & Text-to-CAD](#cadコパイロット--text-to-cad)
- [ジェネレーティブデザイン & トポロジー最適化](#ジェネレーティブデザイン--トポロジー最適化)
- [シミュレーション、CAE & サロゲートAI](#シミュレーションcae--サロゲートai)
- [Physics-ML、PINNs & オープンフレームワーク](#physics-mlpinns--オープンフレームワーク)
- [CAD検索、PDM & ナレッジ](#cad検索pdm--ナレッジ)
- [DFM、GD&T & デザインレビュー](#dfmgdt--デザインレビュー)
- [V&V(検証・妥当性確認)向けAIツール](#vv検証妥当性確認向けaiツール)
- [CAD/デザインツール向けMCPコネクタ](#caddデザインツール向けmcpコネクタ)
- [その他のAwesomeリスト](#その他のawesomeリスト)
- [自動車開発システム向けV&Vツール](#自動車開発システム向けvvツール)
  - [ASAM ODSエコシステム - 主要メンバー & 製品](#asam-odsエコシステム---主要メンバー--製品)
  - [AI支援による大規模V&V(車両~部品、L0-L3)](#ai支援による大規模vv車両部品l0-l3)
- [コントリビューション](#コントリビューション)

---

## CADコパイロット & Text-to-CAD

MCAD内(または隣接)でモデリングを加速する自然言語アシスタントとText-to-CAD。

- [SOLIDWORKS AI Virtual Companions (AURA & LEO)](https://www.solidworks.com/product/solidworks-design/ai-companions) - アプリ内AIコンパニオン。AURAは社内/Webナレッジ、LEOは会話型の設計支援(図面・アセンブリ・フィーチャツリー)。
- [Creo AI Assistant](https://support.ptc.com/help/creo/creo_ai/usascii/ai_assistant/overview.html) - ドキュメント参照、モデル文脈のQ&A、CAD作業支援を行うPTCのCreo向けアシスタント。
- [Autodesk Assistant in Inventor](https://help.autodesk.com/view/INVNTOR/2027/ENU/?guid=ABOUT-AUTODESK-ASSISTANT-INVENTOR) - Inventor向けAutodesk Assistantアドイン。自然言語ヘルプ、モデル照会、タスク自動化。
- [MecAgent](https://mecagent.com/) - SOLIDWORKS & Inventor向けAI CADコパイロット。Text-to-マクロ、図面自動化、工学Q&A、実験的なText-to-STEP/STL。
- [Zoo Design Studio (Zookeeper)](https://zoo.dev/) - 会話型Text-to-CADを備えたAIネイティブCAD(編集可能なB-rep / KCL)。[ドキュメント](https://zoo.dev/docs)。
- [Leo AI](https://www.getleo.ai/) - 機械CAD向けジェネレーティブAI。仕様/スケッチからのアセンブリ生成と形状ベースのパーツ検索。
- [CATIA / 3DEXPERIENCE](https://www.3ds.com/products/catia) - ジオメトリ支援とプラットフォーム知識ワークフロー向けのDassault Systèmes AI機能。
- [Siemens Designcenter NX AI](https://www.siemens.com/en-us/products/designcenter/cad-software/ai/) - AI対応のNX設計。コマンド予測、性能予測、ジェネレーティブ/トポロジーワークフロー。

## ジェネレーティブデザイン & トポロジー最適化

荷重・材料・製法制約に基づく形状生成と軽量化。

- [Autodesk Fusion Generative Design](https://www.autodesk.com/products/fusion-360/) - Fusion内の多目的ジェネレーティブデザイン(CAD/CAM/CAE一体、製造制約付き代替案)。
- [PTC Creo Generative Design](https://www.ptc.com/en/technologies/cad/generative-design) - Creo Generative Topology Optimization (GTO) と Generative Design Extension (GDX)。
- [nTop](https://www.ntop.com/) - ラティス、トポロジー最適化ソリッド、共形流路、AM向け形状のためのフィールド駆動/陰関数設計(旧nTopology)。
- [Simcenter Inspire](https://www.siemens.com/en-us/products/simcenter/mechanical-simulation/inspire/) - 設計者向けトポロジー最適化と構造コンセプト検討(OptiStruct系、旧Altair Inspire)。
- [Ansys GeomAI](https://www.ansys.com/products/ai/geomai) - 参照形状から学習して新コンセプトを探索。SimAI/ソルバーと組み合わせて性能駆動の生成も可能。
- ネイティブCADトポロジー機能 - Fusion、Creo、SOLIDWORKS Simulation、NX Topology Optimizationなどの組み込み軽量化。

## シミュレーション、CAE & サロゲートAI

セットアップ高速化、リアルタイム探索、過去CAEデータからの場予測。

- [Ansys SimAI](https://www.ansys.com/products/ai/simai) - 既存シミュレーション結果でAIを学習し、新設計の3D場を予測(SimAI Proデスクトップ / Premiumクラウド)。
- [Ansys Discovery](https://www.ansys.com/products/3d-design/ansys-discovery) - GPU上でのリアルタイム構造/熱/流体探索。Fluentなど本格ソルバーへの引き継ぎも。
- [Simcenter PhysicsAI](https://www.siemens.com/en-us/products/simcenter/engineering-data-science-ai/physicsai/) - CAEデータ上の幾何深層学習による高速物理予測(旧Altair PhysicsAI)。
- [Neural Concept](https://www.neuralconcept.com/) - 形状ベースのAIによるリアルタイムマルチフィジックス予測と設計空間探索(空力/熱に強み)。
- [SimScale](https://www.simscale.com/) - AI支援セットアップ付きのクラウドCAE(FEA/CFD/熱)で設計エンジニア向けコラボ。

## Physics-ML、PINNs & オープンフレームワーク

自前で学習ループを回すときのオープンな物理情報・データ駆動サロゲート。

- [NVIDIA PhysicsNeMo](https://developer.nvidia.com/physicsnemo) - <span style="color:blue">PINNs、ニューラル演算子、GNN、ハイブリッドPhysics-ML向けのオープンなPyTorchフレームワーク(CFD・構造・EM例あり)。(オープンソース)</span> — [GitHub](https://github.com/NVIDIA/physicsnemo)
- [DeepXDE](https://deepxde.readthedocs.io/) - <span style="color:blue">PINNsやPDE向け深層学習の定番ライブラリ。教育・研究の入口に適する。(オープンソース)</span> — [GitHub](https://github.com/lululxvi/deepxde)

## CAD検索、PDM & ナレッジ

新規形状を作る前に、検証済み部品と社内知を再利用。

- [Leo AI](https://www.getleo.ai/) - 名前や部品番号だけでなく形状でPDM/ボルト内の類似パーツを検索。
- [SOLIDWORKS AURA](https://www.solidworks.com/product/solidworks-design/ai-companions) - 設計環境内で社内ナレッジ、3DSwym、ドキュメントへ接続。

## DFM、GD&T & デザインレビュー

図面/モデルレビュー、変更検出、製造性チェックの自動化。

- [bananaz](https://www.bananaz.ai/) - 機械設計レビュー向けAIエージェント。CAD/図面リビジョン差分、DFM、GD&T/公差レビュー、赤入れ。
- [CoLab AutoReview](https://www.colabsoftware.com/product/autoreview) - モデルと図面のAIデザインレビュー(GD&T、完全性、規格、工程別DFM)と追跡可能なマークアップ。

## V&V(検証・妥当性確認)向けAIツール

物理試作を減らし、シミュレーション根拠を追跡可能にするMLとSPDM。

- [Monolith AI](https://www.monolithai.com/) - 仮想テスト向け機械学習。過去の試験/シミュレーションから結果を予測し、物理プロトタイプを削減。
- [Ansys Minerva](https://www.ansys.com/products/connect/ansys-minerva) - 追跡可能・監査可能なV&Vのためのシミュレーションプロセス&データ管理(SPDM)。
- [Siemens Simcenter Testlab](https://www.siemens.com/en-us/products/simcenter/physical-testing/testlab/) - 物理試験/NVH解析と、試験データからシミュレーションモデルへの相関。
- [COMSOL Model Manager](https://www.comsol.com/model-manager) - V&Vライフサイクル全体でマルチフィジックスモデルを管理・検証・バージョン管理。

## CAD/デザインツール向けMCPコネクタ

AIエージェントがCAD/デザインアプリと対話するためのModel Context Protocolサーバー。

- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) - <span style="color:blue">CAD/デザインベンダー向けMCPコネクタ(Autodesk Fusion MCP / Data MCP、Blender Lab MCP、SketchUpコネクタなど)を含むキュレーションリスト。(オープンソース)</span>

## その他のAwesomeリスト

- [Awesome-Physical-Engineering-AI](https://github.com/010zx00x1/Awesome-Physical-Engineering-AI) - <span style="color:blue">ハードウェアエンジニアリング向けAIツール(CAD、シミュレーション、製造など)。(オープンソース)</span>
- [awesome-ai-cae](https://github.com/kimimgo/awesome-ai-cae) - <span style="color:blue">AI呼び出し可能なCAE/CADツール関連リソース。(オープンソース)</span>
- [awesome-cad-cae](https://github.com/shvyac/awesome-cad-cae) - <span style="color:blue">CAD/CAEアプリ、カーネル、FEA/CFD、トポロジー最適化、TACツール。(オープンソース)</span>
- [awesome-mechanical-engineering](https://github.com/awesomelistsio/awesome-mechanical-engineering) - <span style="color:blue">機械工学向けのより広いツール、プラットフォーム、学習リソース。(オープンソース)</span>

## 自動車開発システム向けV&Vツール

- [dSPACE SCALEXIO / ASM](https://www.dspace.com/) - ECUソフトウェアと車両ダイナミクスを検証するためのHIL(Hardware-in-the-Loop)テストシステムとシミュレーションモデル。
- [Vector CANoe](https://www.vector.com/int/en/products/products-a-z/software/canoe/) - 自動車のVモデル全体でECUおよびネットワークの開発、テスト、解析を行うツール。
- [National Instruments VeriStand](https://www.ni.com/en/shop/veristand.html) - HILシミュレーション、モデル検証、迅速な制御プロトタイピングのためのリアルタイムテストソフトウェア。
- [MathWorks Simulink Test & Requirements Toolbox](https://www.mathworks.com/products/simulink-test.html) - 要求のトレーサビリティを管理し、Simulinkモデルのテストケースに対する検証を自動化。
- [ETAS LABCAR](https://www.etas.com/en/products/labcar.php) - 実際の動作条件下で自動車ECUを検証するHILテスト環境。
- [ASAM ODS (Open Data Services)](https://www.asam.net/standards/detail/ods/) - 欧州の試験データ管理標準で、Vモデル全体にわたる計測・シミュレーション・妥当性確認データの保存と交換を規定。

#### ASAM ODSエコシステム - 主要メンバー & 製品

ASAM ODSベースの試験データ管理製品を開発・保守する主要なASAM e.V.加盟企業。

- [Peak Solution](https://www.peak-solution.com/) - ASAM ODSワーキンググループの活発な貢献企業。プラットフォーム非依存のASAM ODSサーバー[Peak ODS Server (PODS)](https://www.asam.net/members/product-directory/detail/peak-ods-server/)を開発し、openMDMの主要コントリビューターでもある。
- [AVL](https://www.avl.com/) - パワートレインおよび車両の試験データ管理にASAM ODSを対応させた[AVL CONCERTO](https://www.avl.com/)データ解析プラットフォームを提供するOEM/Tier-1試験機器サプライヤー。
- [Vector Informatik](https://www.vector.com/) - ASAM ODSベースのデータ管理・交換機能を備えた計測・キャリブレーションツール(CANape、vSignalyzerなど)を提供するASAM加盟企業。
- [Robert Bosch GmbH](https://www.bosch.com/) - 自動車試験データ管理におけるASAM ODSの要件・ユースケースに貢献するOEM/Tier-1のASAM加盟企業。
- [HighQSoft](https://www.highqsoft.com/) - 試験データ管理システム向けのASAM ODSコンサルティング、データモデル設計、統合サービスを提供するASAM加盟企業。
- [MBBM-VAS](https://www.mbbm-vas.com/) - 計測・試験データ向けの[ASAM ODS & openMDMベースの](https://www.mbbm-vas.com/en/products/data-management/asam-ods)データ管理製品を提供するASAM加盟企業。

### AI支援による大規模V&V(車両~部品、L0-L3)

自動車のVモデル全体を支援するツール群です。左側では車両全体(L0)からシステム(L1)、サブシステム(L2)、部品/コンポーネント(L3)へと要求を分解し、右側では部品レベル(L3)の試験結果を車両全体(L0)の妥当性確認へと積み上げます。

- [Siemens Polarion + Capital](https://www.plm.automation.siemens.com/global/en/products/polarion/) - 車両、システム、サブシステム、部品の各レベルにわたるエンドツーエンドのトレーサビリティを実現するAI支援の要求管理とインパクト分析。
- [PTC Codebeamer X](https://www.ptc.com/en/products/codebeamer) - Vモデル階層全体にわたる要求分解、カバレッジ分析、テストトレーサビリティをAIで支援。
- [Vector PREEvision](https://www.vector.com/int/en/products/products-a-z/software/preevision/) - 車両レベルの要求をシステム、サブシステム、部品の仕様に分解し、V&Vの積み上げのためのトレーサビリティを提供するE/Eシステムエンジニアリングツール。
- [IBM Engineering Lifecycle Management (ELM) with watsonx](https://www.ibm.com/products/engineering-lifecycle-management) - 車両レベルから部品レベルの成果物にまたがる要求分析、変更影響分析、検証トレーサビリティをAIで支援。
- [Ansys medini analyze](https://www.ansys.com/products/safety-analysis/ansys-medini-analyze) - システムレベルのハザードと部品レベルの検証エビデンスを関連付けるモデルベースの安全性・要求分析。

#### オープンソースの代替

車両~部品レベルのVモデル分解と妥当性確認の積み上げという同じ目標を持つオープンソースプロジェクト。

- [Eclipse Capella](https://github.com/eclipse-capella/capella) - <span style="color:blue">Arcadiaメソッドを実装したオープンソースのMBSEツールで、運用・システム・論理・物理レベル(L0-L3)にわたるシステムアーキテクチャの分解を支援。(オープンソース)</span>
- [Eclipse SCORE](https://github.com/eclipse-score/score) - <span style="color:blue">Boschが主導するソフトウェア定義車両向けオープンソースプラットフォームで、車両ソフトウェアスタック全体の要求、アーキテクチャ、V&Vツールを含む。(オープンソース)</span>
- [OpenMBEE](https://github.com/Open-MBEE) - <span style="color:blue">NASA JPLによるオープンソースのモデルベースシステムズエンジニアリング環境で、システムから部品レベルまでの要求とアーキテクチャのトレーサビリティを管理。(オープンソース)</span>
- [Eclipse ProR](https://github.com/eclipse-rmf/org.eclipse.rmf) - <span style="color:blue">ReqIFベースのオープンソース要求管理・トレーサビリティツールで、システムレベル間の要求と検証エビデンスを関連付け。(オープンソース)</span>
- [CARLA](https://github.com/carla-simulator/carla) + [ASAM OpenSCENARIO/OpenDRIVE](https://github.com/esmini/esmini) - <span style="color:blue">部品/シナリオレベルの試験結果を車両全体の妥当性確認に積み上げるためのオープンソース自動運転シミュレータとシナリオ標準。(オープンソース)</span>
- [openMDM](https://openmdm.org/) - <span style="color:blue">ASAM ODS標準をベースにしたEclipse Foundationのオープンソースコンポーネント/コンセプト群で、Vモデル全体にわたる試験・計測・妥当性確認データを管理・交換するシステムを構築できる。(オープンソース)</span>

## コントリビューション

コントリビューションを歓迎します!ツールの追加、リンク切れの修正、新しいカテゴリの提案などは、プルリクエストを開いてください。

**公式/ドキュメントの耐久性のあるURL**、短い説明、実出荷されているツールを優先してください(vaporwareは避けて)。オープンソースは明示してください。

## ライセンス

[LICENSE](LICENSE)を参照してください。
