# Niu 2020 SIP模拟复现核心文献包说明

生成日期：2026-06-25

## 包结构

本目录将 `niu2020_ref` 中当前可见的 59 个参考 PDF 按主题合并为 6 个 PDF 包，并另存 Niu et al. (2020) 主文和 Supporting Information。合并包保留全部源论文页面，并在 PDF 书签中为每篇源论文添加入口。

- PDF 总数：7 个（6 个合并主题包 + 1 个 Niu 2020 主文），小于 30。
- 单个 PDF token 约束：每个 PDF 的文本层粗略估计均低于 2,000,000 tokens。估算采用保守近似 `tokens ~= 文本字符数 / 2.5`。
- SI 文件：`00_Niu_2020_supporting_information.docx`，按原始补充材料格式保存。
- 当前源目录实际整合 PDF：59 个。

## Niu 2020 主文与 SI

- `00_Niu_2020_main_paper_JGR_Solid_Earth.pdf`：18 页，约 70,767 个文本字符，约 28,307 tokens。该文是本复现工作的核心论文，提出三维孔隙尺度 AC3D 框架，用数字岩心计算有效复电导率和介电常数，并区分 interfacial、pore、membrane 及 all polarization 机制。
- `00_Niu_2020_supporting_information.docx`：Niu 2020 补充材料，保留与模型参数、数据、公式或图件说明相关的辅助信息；后续复现参数应优先与主文和 SI 交叉核对。

## 合并 PDF 包概览

| PDF | 主题 | 源论文数 | 页数 | 文本字符数 | 估计tokens |
|---|---|---:|---:|---:|---:|
| `01_foundations_interfacial_edl_membrane_polarization.pdf` | 基础理论：界面极化、电双层、膜极化与表面电导 | 11 | 334 | 735,862 | 294,345 |
| `02_edl_stern_surface_chemistry_parameterization.pdf` | EDL/Stern层、表面化学和复电导参数化 | 15 | 204 | 892,340 | 356,936 |
| `03_pore_scale_simulation_and_digital_rock_workflow.pdf` | 孔隙尺度模拟与数字岩心工作流 | 8 | 118 | 518,718 | 207,488 |
| `04_pnm_reactive_transport_microstructure_evolution.pdf` | 孔隙网络、多相流与微结构演化 | 5 | 64 | 252,150 | 100,860 |
| `05_pore_size_permeability_sip_porosimetry_validation.pdf` | 孔径/孔喉、渗透率、SIP porosimetry 与验证 | 12 | 257 | 816,454 | 326,582 |
| `06_background_reviews_duplicates_and_lkc_context.pdf` | 背景综述、LKC地质背景与重复副本 | 8 | 478 | 866,359 | 346,544 |

## 逐包与逐篇说明

### `01_foundations_interfacial_edl_membrane_polarization.pdf`

- 主题：基础理论：界面极化、电双层、膜极化与表面电导
- 复现用途：支撑 Niu 2020 中 interfacial / pore / membrane 机制拆分的理论根基。
- 包含源论文：11 篇；总页数：334；估计 tokens：294,345

| 序号 | 源PDF | 起始页 | 页数 | 内容速览 | 对复现的作用 |
|---:|---|---:|---:|---|---|
| 1 | `1942_Archie_10_2118_942054_g.pdf` | 1 | 191 | PDF 为老论文汇编/扫描页，文本层较弱但可读到核心脉络。论文建立地层电阻率、孔隙水电阻率、孔隙度和含水饱和度之间的经验关系，即后续 Archie law 的来源。 | 给本项目提供低频/直流体电导基线：在没有表面导电和极化时，孔隙结构通过 formation factor 控制有效电导。 |
| 2 | `1959_marshall_madden_1959_10.1190_1.1438659.pdf` | 192 | 27 | 正文从矿物-电解质界面的电化学极化、离子迁移和孔隙介质中的电荷积累解释 IP 响应。 | 为 SIP 低频虚部/相位来源提供早期理论背景，可帮助区分金属矿物极化与非金属多孔介质极化。 |
| 3 | `1960_Hanai_10_1007_bf01520320.pdf` | 219 | 9 | 论文推导球形分散体系的界面极化介电频散，指出 Maxwell 理论对实际乳状液存在限制，并发展适用于高浓度分散体系的理论。 | 是 interfacial/Maxwell-Wagner 极化的重要理论源头，可用于解释相界面电导率和介电常数差异导致的频散。 |
| 4 | `1962_Schwarz_10_1021_j100818a067.pdf` | 228 | 7 | 论文把低频介电频散归因于外电场驱动反离子气氛/双电层的极化，给出球形颗粒的简化理论，并得到弛豫频率与颗粒半径平方反比的扩散控制关系。 | 是 pore polarization/EDL 极化的核心理论来源，可直接支撑 tau ~ r^2/D 类参数化。 |
| 5 | `1983_Bussian_10_1190_1_1441549.pdf` | 235 | 11 | 正文将 Hanai-Bruggeman 方程扩展到导电岩石骨架浸没于水相的两组分模型，并讨论低频极限与砂岩实验/理论的关系。 | 可作为 effective complex conductivity 与 formation factor/表面导电模型的基础参考。 |
| 6 | `1983_Shilov_10_1016_s0022_0728_83_80251_4.pdf` | 246 | 21 | 论文修正 Schwarz 理论，区分 Stern 层束缚反离子极化与 diffuse layer 浓差极化对低频介电增量的贡献。 | 对区分 Stern-layer polarization 与 diffuse-layer polarization 很关键，可支撑 Niu 2020 后续双电层机制解释。 |
| 7 | `1984_J_10_1190_1_1441755.pdf` | 267 | 21 | 正文把 shaly sands 的 IP 解释为 clay counterion displacement 与 membrane blockage 两类机制，并建立与 CEC、盐度、含油饱和度相关的复电导参数。 | 是 membrane polarization/页岩砂表面导电解释的核心实验-理论文献。 |
| 8 | `1992_delima_sharma_10.1190_1.1443257.pdf` | 288 | 10 | 论文发展广义 Maxwell-Wagner 框架解释 shaly sands 的 membrane polarization，把孔隙/黏土界面、电解质和表面电导联系到复电导响应。 | 对本项目 membrane 机制拆分和窄孔/黏土表面导电建模很重要。 |
| 9 | `1997_Cheng_10_1098_rspa_1997_0009.pdf` | 298 | 18 | 论文用 Rayleigh 方法计算周期球阵列在界面热阻/界面电阻存在时的有效电导，并给出简单、体心、面心立方阵列基准。 | 可作为界面电阻边界条件和有效性质求解器的解析/半解析 benchmark。 |
| 10 | `1998_Glover_10_1029_98gl00296.pdf` | 316 | 4 | 正文讨论表面电导的物理来源、矿物表面电荷和孔隙水电导率对整体电导的影响。 | 可为水相电导、表面电导和 formation factor 的参数范围提供约束。 |
| 11 | `1999_chelidze_gueguen_10.1046_j.1365-246x.1999.00799.x.pdf` | 320 | 15 | 论文系统回顾电谱/复电导理论模型，包括 Maxwell-Wagner、膜极化、双电层和孔隙结构控制的频散。 | 适合作为 SIP 机制综述入口，帮助把不同模型放到同一分类框架。 |

### `02_edl_stern_surface_chemistry_parameterization.pdf`

- 主题：EDL/Stern层、表面化学和复电导参数化
- 复现用途：用于确定盐度、pH、表面电导、Stern/diffuse layer 和水相电导率对复电导率谱的影响。
- 包含源论文：15 篇；总页数：204；估计 tokens：356,936

| 序号 | 源PDF | 起始页 | 页数 | 内容速览 | 对复现的作用 |
|---:|---|---:|---:|---|---|
| 1 | `1999_Delgado_10_1006_jcis_1998_5914.pdf` | 1 | 6 | 正文比较标准模型与含 Stern layer conductance 的模型，指出大颗粒和较高离子强度下 Stern 层切向传导可显著改善低频介电频散解释。 | 可用于解释粒径、ka 和 Stern 层表面电导如何改变 pore/particle polarization。 |
| 2 | `2001_Frye_10_1029_2000jb900392.pdf` | 7 | 12 | 正文测量 Berea sandstone 在不同 NaCl 浓度和 pH 下 10^-3 到 10^6 Hz 的复电导和时域 IP，发现归一化 IP 参数与表面极化相关，并随盐度和 pH 变化。 | 与 Niu 2020 Berea 复现高度相关，可作为孔隙水电导率、pH/盐度敏感性和表面极化解释的实验约束。 |
| 3 | `2001_Grosse_10_1016_s0927_7757_01_00729_4.pdf` | 19 | 13 | 论文把 Dukhin-Shilov 薄双电层理论扩展到宽频范围，并纳入 stagnant layer surface conductivity，覆盖低频和 Maxwell-Wagner-OKonski 频散。 | 可为 EDL 极化、表面电导和宽频复介电响应之间的耦合提供理论依据。 |
| 4 | `2002_titov_komarov_tarasov_levitski_10.1016_S0926-9851(02)00168-4.pdf` | 32 | 17 | 正文结合时域 IP 实验和理论模型，讨论水饱和砂中极化弛豫与孔隙/表面过程的关系。 | 可作为频域 SIP 与时域 IP 转换、弛豫时间解释的补充。 |
| 5 | `2006_Ntarlagiannis_10_1190_1_2187707.pdf` | 49 | 5 | 正文研究 metal-sand 和 clay-sand mixtures 中 IP 响应与表面积之间的关系，显示极化强度可追踪可极化表面或黏土表面。 | 可用于孔极化/表面面积参数化和实验解释。 |
| 6 | `2008_Florsch_10_1029_2007jb005539.pdf` | 54 | 9 | 正文提出黏土岩低频电极化模型，关联表面电导、CEC、孔隙水化学和频率响应。 | 对膜极化/表面导电在含黏土体系中的参数化有用。 |
| 7 | `2008_Leroy_10_1016_j_jcis_2007_12_031.pdf` | 63 | 15 | 论文研究水饱和玻璃珠堆复电导，连接可控颗粒体系、表面电导和双电层极化。 | 适合作为干净颗粒体系的 pore polarization benchmark。 |
| 8 | `2010_Cosenza_10_1111_j_1365_246x_2009_04426_x.pdf` | 78 | 15 | 论文从机制角度研究部分饱和 clay-rocks 的 SIP 响应，关注含水状态、表面过程和极化弛豫。 | 对非饱和/黏土样品机制讨论有价值。 |
| 9 | `2012_Revil_10_1029_2011wr011260.pdf` | 93 | 23 | 论文建立 shaly sands 的 SIP 模型，强调电双层、表面电导和极化机制对复电导的贡献。 | 对含黏土/膜极化机制和水化学参数化很关键。 |
| 10 | `2012_Slater_10_1190_geo2012_0030_1.pdf` | 116 | 14 | 论文汇总砂岩和未固结样品，分析 imaginary conductivity 随孔隙水电导率的规律，并与 diffuse-layer 与 Stern-layer polarization 模型比较。 | 可用于选择水相电导率范围、表面极化幅值和盐度敏感性参数。 |
| 11 | `2013_bucker_hordt_2013a_10.1093_gji_ggt136.pdf` | 130 | 10 | 论文以孔径和电双层参数显式参数化 membrane polarization，提供可解析的频散模型。 | 对本项目 membrane 分量的公式审计和参数敏感性分析很有用。 |
| 12 | `2013_bucker_hordt_2013b_10.1190_geo2012-0548.1.pdf` | 140 | 16 | 论文比较 long narrow pore 与 short narrow pore 模型，分析几何尺度如何影响膜极化谱。 | 可用于把 pnextract 孔喉长度/孔径映射到 membrane relaxation time。 |
| 13 | `2016_bairlein_bucker_hordt_hinze_10.1093_gji_ggw027.pdf` | 156 | 14 | 论文结合实验和 membrane polarization theory 分析 SIP 数据的温度依赖。 | 可用于温度敏感性、扩散系数和离子迁移率参数修正。 |
| 14 | `2018_Joly_10_1016_j_cocis_2018_08_001.pdf` | 170 | 13 | 论文讨论表面电荷实验表征与分子模拟耦合的必要性。 | 可为 zeta potential、surface charge density、Stern 层参数的物理约束提供背景。 |
| 15 | `2019_bucker_flores-orozco_undorf_kemna_10.1029_2019JB017679.pdf` | 183 | 22 | 论文分析 porous media 中 Stern-layer 和 diffuse-layer polarization 的相对贡献。 | 对本项目区分 pore polarization 子机制和参数敏感性很重要。 |

### `03_pore_scale_simulation_and_digital_rock_workflow.pdf`

- 主题：孔隙尺度模拟与数字岩心工作流
- 复现用途：支撑 Berea 三维数字岩心、有效性质计算和 AC2D/AC3D 场求解工作流。
- 包含源论文：8 篇；总页数：118；估计 tokens：207,488

| 序号 | 源PDF | 起始页 | 页数 | 内容速览 | 对复现的作用 |
|---:|---|---:|---:|---|---|
| 1 | `2007_Torres_Verd_n_10_1190_1_2561301.pdf` | 1 | 14 | 论文在二维孔隙图上求解宽频介电/电导响应，比较 EMT 与显式 pore-map 模拟，指出孔隙连通性会影响频散幅度和形状。 | 是本项目 AC2D/AC3D 场求解最直接的前置文献之一，可用于验证边界条件、有效参数反演和频散曲线。 |
| 2 | `2013_M_10_1016_j_cageo_2012_09_008.pdf` | 15 | 11 | 正文用分割 3D 岩心图像计算渗透率、电阻率和弹性模量，比较多种数值方法、边界条件、分辨率和 REV 影响。 | 对验证 AC3D 有效电导求解器、体素分辨率和边界条件非常重要。 |
| 3 | `2013_P_10_1016_j_advwatres_2012_03_003.pdf` | 26 | 20 | 论文综述 micro-CT 成像、分割、孔隙网络提取、直接数值模拟、多相流和上尺度挑战。 | 可指导数字岩心到 PNM/场求解的完整 workflow。 |
| 4 | `2013_Wiegmann_10_1016_j_cageo_2012_09_005.pdf` | 46 | 8 | 正文发布 Fontainebleau、Berea、vuggy carbonate 和 sphere pack 的 benchmark 图像，并讨论不同分割对孔隙结构的影响。 | 对 Berea 数字岩心输入、分割不确定性和 benchmark 数据选择有直接指导。 |
| 5 | `2016_Hoorebeke_10_1016_j_advwatres_2015_05_012.pdf` | 54 | 25 | 论文展示快速实验室 micro-CT 在 pore-scale research 中的能力、局限和未来方向。 | 可指导 CT 图像质量、分辨率、扫描策略和数字岩心输入可信度。 |
| 6 | `2016_Karimpouli_10_1190_geo2015_0260_1.pdf` | 79 | 13 | 论文提出 conditional reconstruction 作为 digital rock physics 的替代策略，用有限图像/统计信息重建孔隙结构。 | 可作为样品图像不完整或需要统计重建时的候选方法。 |
| 7 | `2017_Niu_10_3997_1873_0604_2017055.pdf` | 92 | 10 | 论文提出孔隙尺度数值方法，把电双层影响通过 complex surface conductance 转成固体或孔隙水的 apparent volumetric complex conductivity，再用有限差分求有效复电导。 | 是本项目 Niu 2020 AC3D 复现和机制拆分的直接前置方法论文。 |
| 8 | `2017_Wang_10_1093_gji_ggx140.pdf` | 102 | 17 | 正文用数值方法研究 drained triaxial compression 下 granular materials 的 fabric anisotropy 与 electrical conductivity anisotropy。 | 对各向异性样品和方向性有效电导计算有参考价值。 |

### `04_pnm_reactive_transport_microstructure_evolution.pdf`

- 主题：孔隙网络、多相流与微结构演化
- 复现用途：支撑 pnextract/PNM 几何统计、反应/溶蚀引起的孔隙结构演化和多相扩展。
- 包含源论文：5 篇；总页数：64；估计 tokens：100,860

| 序号 | 源PDF | 起始页 | 页数 | 内容速览 | 对复现的作用 |
|---:|---|---:|---:|---|---|
| 1 | `1953_Burdine_10_2118_225_g.pdf` | 1 | 8 | 正文讨论如何从毛管压力或孔径分布推导相对渗透率，强调孔喉尺度分布与流动能力之间的积分关系。 | 可作为孔隙网络几何分布和渗透率/电学弛豫时间对比的经典背景，不直接给 SIP 方程。 |
| 2 | `2008_Al_Kharusi_10_1029_2006wr005695.pdf` | 9 | 14 | 论文从碳酸盐孔隙图像提取孔隙网络并预测多相流性质，强调网络模型对复杂孔隙空间的适用性和限制。 | 可指导 pnextract/PNM 几何统计、网络参数和多相扩展。 |
| 3 | `2016_Mahabadi_10_1002_2016gc006372.pdf` | 23 | 12 | 正文用 pore-network model 研究 hydrate-bearing sediments 的水 retention curve 和 relative permeability。 | 对 PNM 框架和多相/水合物场景有用，和 SIP 主线间接。 |
| 4 | `2017_Keehm_10_1002_2017jb013972.pdf` | 35 | 15 | 正文通过数值溶蚀模拟研究 tight carbonates 中微结构和渗透率演化。 | 对本项目微流控/方解石溶蚀 AC2D 验证方向很有参考价值。 |
| 5 | `2019_Zhang_10_1029_2018wr024174.pdf` | 50 | 15 | 正文研究矿物 precipitation/dissolution 改变孔隙结构时的 permeability prediction。 | 对反应输运/溶蚀导致孔隙结构演化后再做 SIP 正演很有用。 |

### `05_pore_size_permeability_sip_porosimetry_validation.pdf`

- 主题：孔径/孔喉、渗透率、SIP porosimetry 与验证
- 复现用途：用于把模拟复电导率谱与孔径分布、MICP、NMR、渗透率和实验谱联系起来。
- 包含源论文：12 篇；总页数：257；估计 tokens：326,582

| 序号 | 源PDF | 起始页 | 页数 | 内容速览 | 对复现的作用 |
|---:|---|---:|---:|---|---|
| 1 | `2003_Scott_10_1029_2003gl016951.pdf` | 1 | 4 | 论文把低频电谱特征与 Permo-Triassic sandstone 的孔喉尺度联系起来。 | 对从 SIP 谱反推 pore-throat size 的解释链很有用。 |
| 2 | `2005_Fukes_10_1029_2005wr004202.pdf` | 5 | 13 | 正文围绕饱和/非饱和砂岩的 SIP 与水力参数关系，讨论含水状态、孔隙结构和谱参数对渗透性的指示。 | 用于把复电导谱参数与水力性质联系起来，但需要结合具体样品参数再用于模型。 |
| 3 | `2010_A_10_1111_j_1365_246x_2010_04573_x.pdf` | 18 | 19 | 正文把谱诱导极化的特征时间/极化幅值与颗粒介质渗透率联系起来，讨论孔径或颗粒尺度对弛豫的控制。 | 可用于从模拟谱参数向 permeability 解释桥接。 |
| 4 | `2010_Nordsiek_10_1190_1_3471577.pdf` | 37 | 8 | 论文整理多组砂岩和未固结沉积物数据，发现 imaginary conductivity 与 S_por 之间存在稳健线性关系，并比较不同 IP 参数。 | 可用于把模拟虚部/极化强度转化为比表面积或孔隙结构指标。 |
| 5 | `2012_Revil_10_1029_2011wr011561.pdf` | 45 | 7 | 正文比较 clean sands/sandstones 中 IP 弛豫时间与颗粒尺寸、孔径之间的关系。 | 直接服务于“弛豫时间由 pore radius 还是 grain size 控制”的机制判断。 |
| 6 | `2013_Revil_10_1029_2012wr012700.pdf` | 52 | 22 | 论文给出宽频范围内非饱和多孔材料有效电导和介电常数模型，包含低频极化和高频介电响应。 | 可作为 all-mechanism 宽频复电导/介电常数模型的参考框架。 |
| 7 | `2014_Florsch_10_1093_gji_ggu180.pdf` | 74 | 18 | 论文发展用 SIP 谱反演孔隙尺度分布的 porosimetry 思路，连接弛豫时间分布和孔隙结构。 | 是把模拟 SIP 谱与 pore/throat distribution 对比的核心参考。 |
| 8 | `2014_Torres_Verd_n_10_1190_geo2014_0036_1.pdf` | 92 | 18 | 正文围绕 Fontainebleau sandstone，结合电导、IP 和渗透率讨论孔隙结构控制。 | 可作为干净砂岩体系的实验对照，和 Berea/Niu 结果互补。 |
| 9 | `2015_Kessouri_10_1002_2015wr017074.pdf` | 110 | 70 | 正文将 complex conductivity spectra 的 characteristic relaxation time 与 intrinsic formation factor 联合用于渗透率预测。 | 对从 AC3D 结果推导 permeability 具有直接价值。 |
| 10 | `2016_Binley_10_1002_2015wr018472.pdf` | 180 | 45 | 正文把 complex conductivity 与 NMR 联合用于 sandstone pore geometry 和 permeability prediction。 | 对 LKC/碳酸盐或砂岩样品的 NMR-SIP 联合解释有用。 |
| 11 | `2016_Niu_10_1190_geo2015_0072_1.pdf` | 225 | 16 | 论文用颗粒/孔隙分布卷积 Warburg 模型解释 SIP quadrature conductivity，并把 MICP 转换为孔径分布。 | 是 Niu 2020 之前连接孔径分布和 SIP 谱的关键理论/经验桥梁。 |
| 12 | `2018_Rose_10_1002_2017wr022034.pdf` | 241 | 17 | 正文讨论用 polarization magnitude 和 relaxation time 从 complex conductivity measurements 预测 permeability。 | 可把模拟输出的幅值/时间常数转成渗透率解释。 |

### `06_background_reviews_duplicates_and_lkc_context.pdf`

- 主题：背景综述、LKC地质背景与重复副本
- 复现用途：保留近地表 SIP 综述、LKC 地质背景和已识别重复论文副本，便于追溯但不作为模拟公式核心。
- 包含源论文：8 篇；总页数：478；估计 tokens：346,544

| 序号 | 源PDF | 起始页 | 页数 | 内容速览 | 对复现的作用 |
|---:|---|---:|---:|---|---|
| 1 | `1980_Watney_10_17161_kgsbulletin_no_220_21159.pdf` | 1 | 80 | 该 PDF 基本为扫描版，文本层不可读；从可见题录和页数看是 LKC 地层旋回沉积、沉积相和油气勘探 guidebook。 | 对样品地质背景有用，但不直接提供 SIP 正演方程。 |
| 2 | `1989_French_Sequence_Stratigraphic_Interpretations_and_Modeling_of.pdf` | 81 | 214 | 正文是 Lansing-Kansas City Groups 野外指南，包含旋回地层、岩相、碳酸盐沉积和区域地质解释。 | 可支撑 LKC/Kansas carbonate 样品背景，不直接进入 SIP 数值模型。 |
| 3 | `2000_Friedman_10_1029_2000wr900198.pdf` | 295 | 13 | 论文讨论椭球颗粒取向、形状各向异性和随机/定向排列对复介电性质的影响。 | 可作为颗粒形状和各向异性影响 Maxwell-Wagner 背景频散的参考。 |
| 4 | `2006_Chen_10_1029_2005wr004590.pdf` | 308 | 14 | 论文讨论温度、电解质电导率和相界面对土壤复介电常数的影响，强调 Maxwell-Wagner 极化在低频/中频介电响应中的作用。 | 可支撑 interfacial polarization 背景项和温度/盐度敏感性解释。 |
| 5 | `2006_Or_10_1029_2005wr004744.pdf` | 322 | 9 | 正文讨论几何因子、相连通性和界面过程如何影响部分饱和多孔介质复介电常数。 | 对 AC2D/AC3D 扩展到非饱和或多相状态时有参考价值。 |
| 6 | `2012_L_10_3997_1873_0604_2012027.pdf` | 331 | 60 | 正文综述 SIP 的测量、反演、实验和近地表应用，覆盖仪器、数据处理和物性解释。 | 适合作为项目文献综述和实验-模拟衔接的总入口。 |
| 7 | `2014_Revil_10_1093_gji_ggu180_5556.pdf` | 391 | 18 | 该 PDF 与 2014_Florsch_10_1093_gji_ggu180.pdf 内容相同或高度重复。 | 保留一个即可满足阅读；若后续人工清理，可把重复副本列为候选。 |
| 8 | `2015_Mejus_Predicting_permeability_from_the_characteristic_relaxa.pdf` | 409 | 70 | 该 PDF 与 2015_Kessouri_10_1002_2015wr017074.pdf 内容相同或为同一论文的另一个文件名。 | 后续只需保留一个副本即可。 |

## 使用建议

1. 复现 Niu 2020 时，先读 `00_Niu_2020_main_paper_JGR_Solid_Earth.pdf` 和 `00_Niu_2020_supporting_information.docx`。
2. 机制公式和参数来源优先查 `01_foundations_interfacial_edl_membrane_polarization.pdf` 与 `02_edl_stern_surface_chemistry_parameterization.pdf`。
3. AC2D/AC3D 和数字岩心流程优先查 `03_pore_scale_simulation_and_digital_rock_workflow.pdf`。
4. PNM、多相流和孔隙结构演化优先查 `04_pnm_reactive_transport_microstructure_evolution.pdf`。
5. 与孔径分布、MICP、NMR、渗透率和实验校验相关内容优先查 `05_pore_size_permeability_sip_porosimetry_validation.pdf`。
6. LKC 地质背景、综述和重复副本放在 `06_background_reviews_duplicates_and_lkc_context.pdf`，不是主模拟公式来源。