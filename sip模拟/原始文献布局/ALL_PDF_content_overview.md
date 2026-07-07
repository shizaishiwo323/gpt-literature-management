# niu2020_ref PDF论文内容速览

生成日期：2026-06-25

## 说明

本文件逐个读取 `niu2020_ref` 目录内 PDF 的文本层后整理，重点说明每篇论文的研究对象、主要方法/结论，以及对本项目 SIP/复电导率模拟、孔隙网络、数字岩心和机制拆分的用处。

除 `1980_Watney_10_17161_kgsbulletin_no_220_21159.pdf` 为扫描版、文本层基本不可读外，其余 PDF 均可抽取正文文本。若两个文件为同一论文的重复副本，已在条目中标注。

## 快速分组

- SIP/复电导率和极化机制核心：Hanai 1960、Schwarz 1962、Bussian 1983、Shilov et al. 1983、Vinegar & Waxman 1984、de Lima & Sharma 1992、Chelidze & Gueguen 1999、Lesmes & Frye 2001、Niu & Zhang 2017。
- 电双层/Stern层/表面电导参数：Schwarz 1962、Shilov et al. 1983、Arroyo et al. 1999、Grosse/Shilov et al. 2001、Leroy et al. 2008、Revil 2012、Slater/Weller et al. 2012、Bucker et al. 2019。
- 数字岩心/孔隙网络/有效性质：Dong & Blunt 2009、Al-Kharusi & Blunt 2008、Blunt et al. 2013、Andrae et al. 2013 Part I/II、Bultreys et al. 2016、Karimpouli & Tahmasebi 2016。
- 与渗透率/孔径分布联动：Burdine 1953、Scott & Barker 2003、Weller et al. 2010、Revil et al. 2012、Kessouri et al. 2015、Niu & Revil 2016、Rose et al. 2018。

## 逐篇速览

### 1. Archie, 1942

- 文件：`1942_Archie_10_2118_942054_g.pdf`
- 主题：电阻率测井与 formation factor
- 内容速览：PDF 为老论文汇编/扫描页，文本层较弱但可读到核心脉络。论文建立地层电阻率、孔隙水电阻率、孔隙度和含水饱和度之间的经验关系，即后续 Archie law 的来源。
- 对本项目的用处：给本项目提供低频/直流体电导基线：在没有表面导电和极化时，孔隙结构通过 formation factor 控制有效电导。

### 2. Burdine, 1953

- 文件：`1953_Burdine_10_2118_225_g.pdf`
- 主题：由孔径分布估算相对渗透率
- 内容速览：正文讨论如何从毛管压力或孔径分布推导相对渗透率，强调孔喉尺度分布与流动能力之间的积分关系。
- 对本项目的用处：可作为孔隙网络几何分布和渗透率/电学弛豫时间对比的经典背景，不直接给 SIP 方程。

### 3. Marshall & Madden, 1959

- 文件：`1959_marshall_madden_1959_10.1190_1.1438659.pdf`
- 主题：诱导极化成因
- 内容速览：正文从矿物-电解质界面的电化学极化、离子迁移和孔隙介质中的电荷积累解释 IP 响应。
- 对本项目的用处：为 SIP 低频虚部/相位来源提供早期理论背景，可帮助区分金属矿物极化与非金属多孔介质极化。

### 4. Hanai, 1960

- 文件：`1960_Hanai_10_1007_bf01520320.pdf`
- 主题：界面极化与乳状液介电频散
- 内容速览：论文推导球形分散体系的界面极化介电频散，指出 Maxwell 理论对实际乳状液存在限制，并发展适用于高浓度分散体系的理论。
- 对本项目的用处：是 interfacial/Maxwell-Wagner 极化的重要理论源头，可用于解释相界面电导率和介电常数差异导致的频散。

### 5. Schwarz, 1962

- 文件：`1962_Schwarz_10_1021_j100818a067.pdf`
- 主题：胶体颗粒低频介电频散
- 内容速览：论文把低频介电频散归因于外电场驱动反离子气氛/双电层的极化，给出球形颗粒的简化理论，并得到弛豫频率与颗粒半径平方反比的扩散控制关系。
- 对本项目的用处：是 pore polarization/EDL 极化的核心理论来源，可直接支撑 tau ~ r^2/D 类参数化。

### 6. Watney, 1980

- 文件：`1980_Watney_10_17161_kgsbulletin_no_220_21159.pdf`
- 主题：Lansing-Kansas City 旋回沉积与油气勘探背景
- 内容速览：该 PDF 基本为扫描版，文本层不可读；从可见题录和页数看是 LKC 地层旋回沉积、沉积相和油气勘探 guidebook。
- 对本项目的用处：对样品地质背景有用，但不直接提供 SIP 正演方程。

### 7. Bussian, 1983

- 文件：`1983_Bussian_10_1190_1_1441549.pdf`
- 主题：多孔介质电导模型
- 内容速览：正文将 Hanai-Bruggeman 方程扩展到导电岩石骨架浸没于水相的两组分模型，并讨论低频极限与砂岩实验/理论的关系。
- 对本项目的用处：可作为 effective complex conductivity 与 formation factor/表面导电模型的基础参考。

### 8. Lyklema, Dukhin & Shilov, 1983

- 文件：`1983_Shilov_10_1016_s0022_0728_83_80251_4.pdf`
- 主题：双电层弛豫与低频介电频散
- 内容速览：论文修正 Schwarz 理论，区分 Stern 层束缚反离子极化与 diffuse layer 浓差极化对低频介电增量的贡献。
- 对本项目的用处：对区分 Stern-layer polarization 与 diffuse-layer polarization 很关键，可支撑 Niu 2020 后续双电层机制解释。

### 9. Vinegar & Waxman, 1984

- 文件：`1984_J_10_1190_1_1441755.pdf`
- 主题：页岩砂诱导极化
- 内容速览：正文把 shaly sands 的 IP 解释为 clay counterion displacement 与 membrane blockage 两类机制，并建立与 CEC、盐度、含油饱和度相关的复电导参数。
- 对本项目的用处：是 membrane polarization/页岩砂表面导电解释的核心实验-理论文献。

### 10. French & Franseen, 1989

- 文件：`1989_French_Sequence_Stratigraphic_Interpretations_and_Modeling_of.pdf`
- 主题：LKC 旋回层序地层解释
- 内容速览：正文是 Lansing-Kansas City Groups 野外指南，包含旋回地层、岩相、碳酸盐沉积和区域地质解释。
- 对本项目的用处：可支撑 LKC/Kansas carbonate 样品背景，不直接进入 SIP 数值模型。

### 11. de Lima & Sharma, 1992

- 文件：`1992_delima_sharma_10.1190_1.1443257.pdf`
- 主题：页岩砂膜极化的 Maxwell-Wagner 理论
- 内容速览：论文发展广义 Maxwell-Wagner 框架解释 shaly sands 的 membrane polarization，把孔隙/黏土界面、电解质和表面电导联系到复电导响应。
- 对本项目的用处：对本项目 membrane 机制拆分和窄孔/黏土表面导电建模很重要。

### 12. Cheng & Torquato, 1997

- 文件：`1997_Cheng_10_1098_rspa_1997_0009.pdf`
- 主题：带界面阻抗球阵列有效电导
- 内容速览：论文用 Rayleigh 方法计算周期球阵列在界面热阻/界面电阻存在时的有效电导，并给出简单、体心、面心立方阵列基准。
- 对本项目的用处：可作为界面电阻边界条件和有效性质求解器的解析/半解析 benchmark。

### 13. Glover et al., 1998

- 文件：`1998_Glover_10_1029_98gl00296.pdf`
- 主题：天然砂、砂岩和黏土表面电导
- 内容速览：正文讨论表面电导的物理来源、矿物表面电荷和孔隙水电导率对整体电导的影响。
- 对本项目的用处：可为水相电导、表面电导和 formation factor 的参数范围提供约束。

### 14. Chelidze & Gueguen, 1999

- 文件：`1999_chelidze_gueguen_10.1046_j.1365-246x.1999.00799.x.pdf`
- 主题：多孔岩石电谱理论综述
- 内容速览：论文系统回顾电谱/复电导理论模型，包括 Maxwell-Wagner、膜极化、双电层和孔隙结构控制的频散。
- 对本项目的用处：适合作为 SIP 机制综述入口，帮助把不同模型放到同一分类框架。

### 15. Arroyo, Carrique, Bellini & Delgado, 1999

- 文件：`1999_Delgado_10_1006_jcis_1998_5914.pdf`
- 主题：Stern 层电导与颗粒尺度效应
- 内容速览：正文比较标准模型与含 Stern layer conductance 的模型，指出大颗粒和较高离子强度下 Stern 层切向传导可显著改善低频介电频散解释。
- 对本项目的用处：可用于解释粒径、ka 和 Stern 层表面电导如何改变 pore/particle polarization。

### 16. Friedman, 2000

- 文件：`2000_Friedman_10_1029_2000wr900198.pdf`
- 主题：颗粒形状对有效介电常数的影响
- 内容速览：论文讨论椭球颗粒取向、形状各向异性和随机/定向排列对复介电性质的影响。
- 对本项目的用处：可作为颗粒形状和各向异性影响 Maxwell-Wagner 背景频散的参考。

### 17. Lesmes & Frye, 2001

- 文件：`2001_Frye_10_1029_2000jb900392.pdf`
- 主题：Berea 砂岩孔隙流体化学对复电导/IP 的影响
- 内容速览：正文测量 Berea sandstone 在不同 NaCl 浓度和 pH 下 10^-3 到 10^6 Hz 的复电导和时域 IP，发现归一化 IP 参数与表面极化相关，并随盐度和 pH 变化。
- 对本项目的用处：与 Niu 2020 Berea 复现高度相关，可作为孔隙水电导率、pH/盐度敏感性和表面极化解释的实验约束。

### 18. Shilov, Delgado, Gonzalez-Caballero & Grosse, 2001

- 文件：`2001_Grosse_10_1016_s0927_7757_01_00729_4.pdf`
- 主题：薄双电层宽频介电频散
- 内容速览：论文把 Dukhin-Shilov 薄双电层理论扩展到宽频范围，并纳入 stagnant layer surface conductivity，覆盖低频和 Maxwell-Wagner-OKonski 频散。
- 对本项目的用处：可为 EDL 极化、表面电导和宽频复介电响应之间的耦合提供理论依据。

### 19. Titov et al., 2002

- 文件：`2002_titov_komarov_tarasov_levitski_10.1016_S0926-9851(02)00168-4.pdf`
- 主题：水饱和砂的时域 IP 理论与实验
- 内容速览：正文结合时域 IP 实验和理论模型，讨论水饱和砂中极化弛豫与孔隙/表面过程的关系。
- 对本项目的用处：可作为频域 SIP 与时域 IP 转换、弛豫时间解释的补充。

### 20. Scott & Barker, 2003

- 文件：`2003_Scott_10_1029_2003gl016951.pdf`
- 主题：用低频电谱估算孔喉尺寸
- 内容速览：论文把低频电谱特征与 Permo-Triassic sandstone 的孔喉尺度联系起来。
- 对本项目的用处：对从 SIP 谱反推 pore-throat size 的解释链很有用。

### 21. Kruschwitz et al./相关 WRR 2005

- 文件：`2005_Fukes_10_1029_2005wr004202.pdf`
- 主题：SIP 与砂岩水力性质
- 内容速览：正文围绕饱和/非饱和砂岩的 SIP 与水力参数关系，讨论含水状态、孔隙结构和谱参数对渗透性的指示。
- 对本项目的用处：用于把复电导谱参数与水力性质联系起来，但需要结合具体样品参数再用于模型。

### 22. Chen & Or, 2006

- 文件：`2006_Chen_10_1029_2005wr004590.pdf`
- 主题：Maxwell-Wagner 极化对土壤复介电常数的影响
- 内容速览：论文讨论温度、电解质电导率和相界面对土壤复介电常数的影响，强调 Maxwell-Wagner 极化在低频/中频介电响应中的作用。
- 对本项目的用处：可支撑 interfacial polarization 背景项和温度/盐度敏感性解释。

### 23. Ntarlagiannis & Wishart, 2006

- 文件：`2006_Ntarlagiannis_10_1190_1_2187707.pdf`
- 主题：IP 与比表面积关系
- 内容速览：正文研究 metal-sand 和 clay-sand mixtures 中 IP 响应与表面积之间的关系，显示极化强度可追踪可极化表面或黏土表面。
- 对本项目的用处：可用于孔极化/表面面积参数化和实验解释。

### 24. Chen & Or, 2006

- 文件：`2006_Or_10_1029_2005wr004744.pdf`
- 主题：部分饱和多孔介质几何与界面过程
- 内容速览：正文讨论几何因子、相连通性和界面过程如何影响部分饱和多孔介质复介电常数。
- 对本项目的用处：对 AC2D/AC3D 扩展到非饱和或多相状态时有参考价值。

### 25. Toumelin & Torres-Verdin, 2007

- 文件：`2007_Torres_Verd_n_10_1190_1_2561301.pdf`
- 主题：二维孔隙尺度宽频电磁色散模拟
- 内容速览：论文在二维孔隙图上求解宽频介电/电导响应，比较 EMT 与显式 pore-map 模拟，指出孔隙连通性会影响频散幅度和形状。
- 对本项目的用处：是本项目 AC2D/AC3D 场求解最直接的前置文献之一，可用于验证边界条件、有效参数反演和频散曲线。

### 26. Al-Kharusi & Blunt, 2008

- 文件：`2008_Al_Kharusi_10_1029_2006wr005695.pdf`
- 主题：碳酸盐图像提取网络的多相流预测
- 内容速览：论文从碳酸盐孔隙图像提取孔隙网络并预测多相流性质，强调网络模型对复杂孔隙空间的适用性和限制。
- 对本项目的用处：可指导 pnextract/PNM 几何统计、网络参数和多相扩展。

### 27. Leroy, Revil, Kemna 等/Florsch 相关, 2008

- 文件：`2008_Florsch_10_1029_2007jb005539.pdf`
- 主题：黏土岩低频电极化物理模型
- 内容速览：正文提出黏土岩低频电极化模型，关联表面电导、CEC、孔隙水化学和频率响应。
- 对本项目的用处：对膜极化/表面导电在含黏土体系中的参数化有用。

### 28. Leroy et al., 2008

- 文件：`2008_Leroy_10_1016_j_jcis_2007_12_031.pdf`
- 主题：水饱和玻璃珠堆复电导
- 内容速览：论文研究水饱和玻璃珠堆复电导，连接可控颗粒体系、表面电导和双电层极化。
- 对本项目的用处：适合作为干净颗粒体系的 pore polarization benchmark。

### 29. Revil & Florsch, 2010

- 文件：`2010_A_10_1111_j_1365_246x_2010_04573_x.pdf`
- 主题：由 SIP 确定颗粒介质渗透率
- 内容速览：正文把谱诱导极化的特征时间/极化幅值与颗粒介质渗透率联系起来，讨论孔径或颗粒尺度对弛豫的控制。
- 对本项目的用处：可用于从模拟谱参数向 permeability 解释桥接。

### 30. Cosenza et al., 2010

- 文件：`2010_Cosenza_10_1111_j_1365_246x_2009_04426_x.pdf`
- 主题：部分饱和黏土岩 SIP 机制
- 内容速览：论文从机制角度研究部分饱和 clay-rocks 的 SIP 响应，关注含水状态、表面过程和极化弛豫。
- 对本项目的用处：对非饱和/黏土样品机制讨论有价值。

### 31. Weller, Slater, Nordsiek & Ntarlagiannis, 2010

- 文件：`2010_Nordsiek_10_1190_1_3471577.pdf`
- 主题：IP 参数估算单位孔隙体积比表面积
- 内容速览：论文整理多组砂岩和未固结沉积物数据，发现 imaginary conductivity 与 S_por 之间存在稳健线性关系，并比较不同 IP 参数。
- 对本项目的用处：可用于把模拟虚部/极化强度转化为比表面积或孔隙结构指标。

### 32. Kemna 等, 2012

- 文件：`2012_L_10_3997_1873_0604_2012027.pdf`
- 主题：近地表 SIP 方法综述
- 内容速览：正文综述 SIP 的测量、反演、实验和近地表应用，覆盖仪器、数据处理和物性解释。
- 对本项目的用处：适合作为项目文献综述和实验-模拟衔接的总入口。

### 33. Revil, 2012

- 文件：`2012_Revil_10_1029_2011wr011260.pdf`
- 主题：页岩砂 SIP 与电双层
- 内容速览：论文建立 shaly sands 的 SIP 模型，强调电双层、表面电导和极化机制对复电导的贡献。
- 对本项目的用处：对含黏土/膜极化机制和水化学参数化很关键。

### 34. Revil et al., 2012

- 文件：`2012_Revil_10_1029_2011wr011561.pdf`
- 主题：颗粒尺寸还是孔径控制 IP 弛豫时间
- 内容速览：正文比较 clean sands/sandstones 中 IP 弛豫时间与颗粒尺寸、孔径之间的关系。
- 对本项目的用处：直接服务于“弛豫时间由 pore radius 还是 grain size 控制”的机制判断。

### 35. Weller/Slater 等, 2012

- 文件：`2012_Slater_10_1190_geo2012_0030_1.pdf`
- 主题：盐度对复电导的影响与 EDL 模型比较
- 内容速览：论文汇总砂岩和未固结样品，分析 imaginary conductivity 随孔隙水电导率的规律，并与 diffuse-layer 与 Stern-layer polarization 模型比较。
- 对本项目的用处：可用于选择水相电导率范围、表面极化幅值和盐度敏感性参数。

### 36. Bucker & Hordt, 2013

- 文件：`2013_bucker_hordt_2013a_10.1093_gji_ggt136.pdf`
- 主题：显式孔径和 EDL 参数的膜极化解析模型
- 内容速览：论文以孔径和电双层参数显式参数化 membrane polarization，提供可解析的频散模型。
- 对本项目的用处：对本项目 membrane 分量的公式审计和参数敏感性分析很有用。

### 37. Bucker & Hordt, 2013

- 文件：`2013_bucker_hordt_2013b_10.1190_geo2012-0548.1.pdf`
- 主题：长/短窄孔膜极化模型
- 内容速览：论文比较 long narrow pore 与 short narrow pore 模型，分析几何尺度如何影响膜极化谱。
- 对本项目的用处：可用于把 pnextract 孔喉长度/孔径映射到 membrane relaxation time。

### 38. Andrae et al., 2013 Part II

- 文件：`2013_M_10_1016_j_cageo_2012_09_008.pdf`
- 主题：数字岩心有效性质 benchmark
- 内容速览：正文用分割 3D 岩心图像计算渗透率、电阻率和弹性模量，比较多种数值方法、边界条件、分辨率和 REV 影响。
- 对本项目的用处：对验证 AC3D 有效电导求解器、体素分辨率和边界条件非常重要。

### 39. Blunt et al., 2013

- 文件：`2013_P_10_1016_j_advwatres_2012_03_003.pdf`
- 主题：孔隙尺度成像与建模综述
- 内容速览：论文综述 micro-CT 成像、分割、孔隙网络提取、直接数值模拟、多相流和上尺度挑战。
- 对本项目的用处：可指导数字岩心到 PNM/场求解的完整 workflow。

### 40. Revil, 2013

- 文件：`2013_Revil_10_1029_2012wr012700.pdf`
- 主题：非饱和多孔介质 1 mHz-1 GHz 有效电导与介电常数
- 内容速览：论文给出宽频范围内非饱和多孔材料有效电导和介电常数模型，包含低频极化和高频介电响应。
- 对本项目的用处：可作为 all-mechanism 宽频复电导/介电常数模型的参考框架。

### 41. Andrae et al., 2013 Part I

- 文件：`2013_Wiegmann_10_1016_j_cageo_2012_09_005.pdf`
- 主题：数字岩心成像与分割 benchmark
- 内容速览：正文发布 Fontainebleau、Berea、vuggy carbonate 和 sphere pack 的 benchmark 图像，并讨论不同分割对孔隙结构的影响。
- 对本项目的用处：对 Berea 数字岩心输入、分割不确定性和 benchmark 数据选择有直接指导。

### 42. Revil/Florsch/Camerlynck 等, 2014

- 文件：`2014_Florsch_10_1093_gji_ggu180.pdf`
- 主题：SIP porosimetry
- 内容速览：论文发展用 SIP 谱反演孔隙尺度分布的 porosimetry 思路，连接弛豫时间分布和孔隙结构。
- 对本项目的用处：是把模拟 SIP 谱与 pore/throat distribution 对比的核心参考。

### 43. Revil/Florsch/Camerlynck 等, 2014

- 文件：`2014_Revil_10_1093_gji_ggu180_5556.pdf`
- 主题：SIP porosimetry（重复副本）
- 内容速览：该 PDF 与 2014_Florsch_10_1093_gji_ggu180.pdf 内容相同或高度重复。
- 对本项目的用处：保留一个即可满足阅读；若后续人工清理，可把重复副本列为候选。

### 44. Torres-Verdin et al., 2014

- 文件：`2014_Torres_Verd_n_10_1190_geo2014_0036_1.pdf`
- 主题：Fontainebleau 砂岩电导、IP 与渗透率
- 内容速览：正文围绕 Fontainebleau sandstone，结合电导、IP 和渗透率讨论孔隙结构控制。
- 对本项目的用处：可作为干净砂岩体系的实验对照，和 Berea/Niu 结果互补。

### 45. Kessouri et al., 2015

- 文件：`2015_Kessouri_10_1002_2015wr017074.pdf`
- 主题：由特征弛豫时间和 intrinsic formation factor 预测渗透率
- 内容速览：正文将 complex conductivity spectra 的 characteristic relaxation time 与 intrinsic formation factor 联合用于渗透率预测。
- 对本项目的用处：对从 AC3D 结果推导 permeability 具有直接价值。

### 46. Kessouri et al., 2015

- 文件：`2015_Mejus_Predicting_permeability_from_the_characteristic_relaxa.pdf`
- 主题：渗透率预测论文副本
- 内容速览：该 PDF 与 2015_Kessouri_10_1002_2015wr017074.pdf 内容相同或为同一论文的另一个文件名。
- 对本项目的用处：后续只需保留一个副本即可。

### 47. Bairlein, Bucker, Hordt & Hinze, 2016

- 文件：`2016_bairlein_bucker_hordt_hinze_10.1093_gji_ggw027.pdf`
- 主题：SIP 温度依赖与膜极化理论
- 内容速览：论文结合实验和 membrane polarization theory 分析 SIP 数据的温度依赖。
- 对本项目的用处：可用于温度敏感性、扩散系数和离子迁移率参数修正。

### 48. Binley et al., 2016

- 文件：`2016_Binley_10_1002_2015wr018472.pdf`
- 主题：用复电导和 NMR 估计砂岩孔隙几何参数
- 内容速览：正文把 complex conductivity 与 NMR 联合用于 sandstone pore geometry 和 permeability prediction。
- 对本项目的用处：对 LKC/碳酸盐或砂岩样品的 NMR-SIP 联合解释有用。

### 49. Bultreys, Van Hoorebeke & Cnudde, 2016

- 文件：`2016_Hoorebeke_10_1016_j_advwatres_2015_05_012.pdf`
- 主题：实验室 micro-CT 在孔隙尺度研究中的应用
- 内容速览：论文展示快速实验室 micro-CT 在 pore-scale research 中的能力、局限和未来方向。
- 对本项目的用处：可指导 CT 图像质量、分辨率、扫描策略和数字岩心输入可信度。

### 50. Karimpouli & Tahmasebi, 2016

- 文件：`2016_Karimpouli_10_1190_geo2015_0260_1.pdf`
- 主题：数字岩心条件重建
- 内容速览：论文提出 conditional reconstruction 作为 digital rock physics 的替代策略，用有限图像/统计信息重建孔隙结构。
- 对本项目的用处：可作为样品图像不完整或需要统计重建时的候选方法。

### 51. Mahabadi et al., 2016

- 文件：`2016_Mahabadi_10_1002_2016gc006372.pdf`
- 主题：水合物沉积物水 retention 与相对渗透率 PNM
- 内容速览：正文用 pore-network model 研究 hydrate-bearing sediments 的水 retention curve 和 relative permeability。
- 对本项目的用处：对 PNM 框架和多相/水合物场景有用，和 SIP 主线间接。

### 52. Niu & Revil, 2016

- 文件：`2016_Niu_10_1190_geo2015_0072_1.pdf`
- 主题：复电导谱与 MICP 孔隙分布连接
- 内容速览：论文用颗粒/孔隙分布卷积 Warburg 模型解释 SIP quadrature conductivity，并把 MICP 转换为孔径分布。
- 对本项目的用处：是 Niu 2020 之前连接孔径分布和 SIP 谱的关键理论/经验桥梁。

### 53. Keehm et al., 2017

- 文件：`2017_Keehm_10_1002_2017jb013972.pdf`
- 主题：方解石溶蚀导致的渗透率和微结构演化
- 内容速览：正文通过数值溶蚀模拟研究 tight carbonates 中微结构和渗透率演化。
- 对本项目的用处：对本项目微流控/方解石溶蚀 AC2D 验证方向很有参考价值。

### 54. Niu & Zhang, 2017

- 文件：`2017_Niu_10_3997_1873_0604_2017055.pdf`
- 主题：饱和颗粒材料孔隙尺度复电导建模
- 内容速览：论文提出孔隙尺度数值方法，把电双层影响通过 complex surface conductance 转成固体或孔隙水的 apparent volumetric complex conductivity，再用有限差分求有效复电导。
- 对本项目的用处：是本项目 Niu 2020 AC3D 复现和机制拆分的直接前置方法论文。

### 55. Wang et al., 2017

- 文件：`2017_Wang_10_1093_gji_ggx140.pdf`
- 主题：颗粒材料电导各向异性与织构各向异性
- 内容速览：正文用数值方法研究 drained triaxial compression 下 granular materials 的 fabric anisotropy 与 electrical conductivity anisotropy。
- 对本项目的用处：对各向异性样品和方向性有效电导计算有参考价值。

### 56. Joly et al., 2018

- 文件：`2018_Joly_10_1016_j_cocis_2018_08_001.pdf`
- 主题：表面电荷测量与分子模拟
- 内容速览：论文讨论表面电荷实验表征与分子模拟耦合的必要性。
- 对本项目的用处：可为 zeta potential、surface charge density、Stern 层参数的物理约束提供背景。

### 57. Rose et al., 2018

- 文件：`2018_Rose_10_1002_2017wr022034.pdf`
- 主题：由复电导极化幅值和弛豫时间预测渗透率
- 内容速览：正文讨论用 polarization magnitude 和 relaxation time 从 complex conductivity measurements 预测 permeability。
- 对本项目的用处：可把模拟输出的幅值/时间常数转成渗透率解释。

### 58. Bucker et al., 2019

- 文件：`2019_bucker_flores-orozco_undorf_kemna_10.1029_2019JB017679.pdf`
- 主题：Stern 层与 diffuse layer 极化机制作用
- 内容速览：论文分析 porous media 中 Stern-layer 和 diffuse-layer polarization 的相对贡献。
- 对本项目的用处：对本项目区分 pore polarization 子机制和参数敏感性很重要。

### 59. Zhang et al., 2019

- 文件：`2019_Zhang_10_1029_2018wr024174.pdf`
- 主题：矿物沉淀/溶蚀岩石渗透率数值预测
- 内容速览：正文研究矿物 precipitation/dissolution 改变孔隙结构时的 permeability prediction。
- 对本项目的用处：对反应输运/溶蚀导致孔隙结构演化后再做 SIP 正演很有用。

### 60. Dong & Blunt, 2009

- 文件：`Pore-network extraction from micro-computerized-tomography images.pdf`
- 主题：从 micro-CT 图像提取孔隙网络
- 内容速览：正文提出/说明从三维 micro-CT 孔隙空间图像提取 pore-network 的方法，用网络元素表示孔体和孔喉。
- 对本项目的用处：是本项目 pnextract/球棍网络可视化和孔喉统计的关键方法依据。
