# NMR GPT 项目文献整合说明

本目录把原始 NMR 文献 PDF 整合为 8 个可上传/检索的 PDF 合并卷。合并时保留原始 PDF 页面内容，并在合并 PDF 内加入每篇文献的书签入口。

## 合并 PDF 总览

| 合并PDF | 内容定位 | 文献数 | 页数 | 估算tokens |
|---|---|---:|---:|---:|
| 01_NMR_application_general.pdf | 应用案例：混凝土、矿物、多相流、泥炭、岩石与岩石物理参数估计 | 11 | 159 | 200,822 |
| 02_NMR_application_pore_coupling.pdf | 应用案例：孔隙耦合、非水相流体、MICP/NMR 对比与相关岩石实验 | 7 | 65 | 65,997 |
| 03_NMR_measurement_modeling_2D_maps.pdf | 测量与建模：CPMG、T1-T2、T2-T2、多维 NMR 图谱与反演 | 8 | 207 | 88,119 |
| 04_NMR_simulation_echo_FEM_LBM.pdf | 数值模拟：回波串、FEM/COMSOL、有限体积与 LBM | 11 | 183 | 166,028 |
| 05_NMR_simulation_machine_learning_matrix.pdf | 数值模拟：机器学习、神经网络、committee machine 与矩阵对角化方法 | 10 | 153 | 151,412 |
| 06_NMR_simulation_random_walk.pdf | 数值模拟：随机游走、扩散耦合、内部梯度、冻土/碳酸盐岩应用 | 17 | 382 | 248,132 |
| 07_NMR_theory_review_core.pdf | 理论与综述：NMR 原理、弛豫/扩散机制、近地表/油气应用综述 | 13 | 241 | 228,887 |
| 08_NMR_theory_review_books_Coates_Dunn.pdf | 教材/专著类资料：Coates 与 Dunn 章节/材料 | 14 | 543 | 142,582 |

所有合并卷的估算 token 均低于 2,000,000。估算方法按前两页抽取文本折算，扫描版或图片型 PDF 会按页数保守估算；实际 GPT 计数可能略有差异。

## 每个合并 PDF 的内容

### 01_NMR_application_general.pdf

- 内容：应用案例：混凝土、矿物、多相流、泥炭、岩石与岩石物理参数估计
- 规模：11 个原始 PDF，159 页，估算 200,822 tokens。
- 包含文献/SI：
  - A phenomenological approach on the influence of paramagnetic iron in cement stone on 2D T1-T2 relaxation in single-sided 1H nuclear magnetic resonance (15页；T1-T2 多维 NMR；水泥/混凝土材料应用)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\concrete\1-s2.0-S000888461831038X-main.pdf
  - McDonald2005 (9页；水泥/混凝土材料应用)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\concrete\x_McDonald2005.pdf
  - Paramagnetic Effects of Iron(III) Species on Nuclear Magnetic Relaxation of Fluid Protons in Porous Media (12页；矿物表面/吸附水)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Mineral\Bryar2000.pdf
  - No Job Name (6页；多相流)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Multiphse flow\Daughney2000.pdf
  - Wettability Quantification in Mixed-Wet Rocks Using a New NMR-Based Method (22页；多相流)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Multiphse flow\Tandon2020.pdf
  - Hydraulic conductivity estimation by NMR data in unconsolidated geological materials: insights from SDR model calibrations (16页；泥炭/非固结材料应用；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Peat\Hydraulic conductivity estimation by NMR data in unconsolidated geological materials insights from SDR model calibrations.pdf
  - Nuclear magnetic resonance relaxometry to characterise the decomposition degree of peat soils (14页；泥炭/非固结材料应用；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Peat\Nuclear magnetic resonance relaxometry to characterise the decomposition degree of peat soils.pdf
  - 2015: Comparison of Pore Size Distribution by NMR Relaxation and Nmr Cryoporometry in Shales (12页；岩石物理参数估计)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Petrophysics\Fleury2015.pdf
  - April 2018 Publication PRESS.indd (17页；岩石物理参数估计；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Petrophysics\Jacomoetal2018_Petrophysics.pdf
  - Relaxation mechanisms and shales (22页；岩石物理参数估计)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Petrophysics\Washburn2014.pdf
  - A two-region transport model for interpreting - measurements in complex systems (14页；NMR application)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Rock\Maneval2019.pdf

### 02_NMR_application_pore_coupling.pdf

- 内容：应用案例：孔隙耦合、非水相流体、MICP/NMR 对比与相关岩石实验
- 规模：7 个原始 PDF，65 页，估算 65,997 tokens。
- 包含文献/SI：
  - ANAND.vp (20页；孔隙耦合/扩散耦合)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Pore coupling\Anand2007.pdf
  - A laboratory study of NMR relaxation times and pore coupling in heterogeneous media (7页；孔隙耦合/扩散耦合)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Pore coupling\Grunewald2009_LabStudy_PoreCoupling.pdf
  - SURFACE RELAXIVITY ESTIMATION AND NMR-MICP MATCHING IN DIFFUSIONALY COUPLED ROCKS (6页；孔隙耦合/扩散耦合；扩散与弛豫机制)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Pore coupling\Mesquita2016_MICP.pdf
  - Diffusive coupling in heptane-saturated kerogen isolates evidenced by NMR T1-T2 and T2-T2 maps (10页；孔隙耦合/扩散耦合；T2-T2 多维 NMR；T1-T2 多维 NMR；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Pore coupling\Singer2020_notWater.pdf
  - untitled (5页；孔隙耦合/扩散耦合)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Pore coupling\Song2014_reviewLetters.pdf
  - Detection of intermolecular homonuclear dipolar coupling in organic rich shale by transverse relaxation exchange (7页；孔隙耦合/扩散耦合)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Pore coupling\Washburn2017.pdf
  - Quantitative analysis of diffusional pore coupling from T2-store-T2 NMR experiments (10页；孔隙耦合/扩散耦合；扩散与弛豫机制)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR application\Lab NMR\Pore coupling\x_Fleury2009.pdf

### 03_NMR_measurement_modeling_2D_maps.pdf

- 内容：测量与建模：CPMG、T1-T2、T2-T2、多维 NMR 图谱与反演
- 规模：8 个原始 PDF，207 页，估算 88,119 tokens。
- 包含文献/SI：
  - A new method to establish NMR T2 spectrum based on bimodal Gaussian density function_ A case study of tight sandstone in East China Sea Basin (10页；CPMG/T2 采集或反演)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR measurement and modeling\CPMG T2 map\1-s2.0-S092041051830353X-main.pdf
  - 4199 (150页；T2-T2 多维 NMR)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR measurement and modeling\T2-T2\4199.pdf
  - Monteilheit2006 T2 T2 (10页；T2-T2 多维 NMR)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR measurement and modeling\T2-T2\Monteilheit2006_T2-T2.pdf
  - Johnson2014 (7页；T2-T2 多维 NMR)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR measurement and modeling\T2-T2\x_Johnson2014.pdf
  - Schwartz2013 t2t2 (13页；T2-T2 多维 NMR)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR measurement and modeling\T2-T2\x_Schwartz2013_t2t2.pdf
  - untitled (4页；T2-T2 多维 NMR)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR measurement and modeling\T2-T2\x_Song2008.pdf
  - The robust identification of exchange from T2â€“T2 time-domain features (8页；T2-T2 多维 NMR)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR measurement and modeling\T2-T2\x_Song2016.pdf
  - Characterization of porous media by T2-T2 correlation beyond fast diffusion limit (5页；T2-T2 多维 NMR；扩散与弛豫机制)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR measurement and modeling\T2-T2\Yu_2019.pdf

### 04_NMR_simulation_echo_FEM_LBM.pdf

- 内容：数值模拟：回波串、FEM/COMSOL、有限体积与 LBM
- 规模：11 个原始 PDF，183 页，估算 166,028 tokens。
- 包含文献/SI：
  - Numerical investigating the low field NMR response of representative pores at different pulse sequence parameters (11页；NMR simulation)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Echo train simulation\1-s2.0-S0098300421000686-main.pdf
  - Tan et al. - 2012 - Numerical simulation of (T2, T1) 2D NMR and fluid .pdf (13页；NMR simulation；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Echo train simulation\Tan et al. - 2012 - Numerical simulation of (T2, T1) 2D NMR and fluid .pdf
  - An investigation into the effects of pore connectivity on T2 NMR relaxation (13页；有限元模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\FEM\Ghomeshi2018_FEM.pdf
  - doi:10.1016/S1090-7807(02)00039-3 (10页；有限元模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\FEM\Hagslatt2002_restrictiveGeometries.pdf
  - A finite element approach to forward modeling of nuclear magnetic resonance measurements in coupled pore systems (13页；有限元模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\FEM\Mitchel2019_FEModeling.pdf
  - Microscale Simulations of NMR Relaxation in Porous Media Considering Internal Field Gradients (12页；有限元模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\FEM\Mohnke2010.pdf
  - Oliveira2021 COMSOL Guide! (49页；有限元模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\FEM\Oliveira2021_COMSOL_Guide!.pdf
  - Schwartz2013 t2t2 (13页；有限元模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\FEM\Schwartz2013_t2t2.pdf
  - Effect of Internal Magnetic-Field Gradients on Nuclear-Magnetic-Resonance Measurements and Nuclear-Magnetic-Resonance-Based (18页；有限元模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\FEM\Tandon2018_FiniteVolumeMethod_InternalGradients.pdf
  - USING STANDARD SYSTE (15页；格子 Boltzmann 模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\LBM\Guyer2000_LBM.pdf
  - Joint numerical microscale simulations of multiphase flow and NMR relaxation behavior in porous media using Lattice Boltzmann methods (16页；格子 Boltzmann 模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\LBM\Mohnke2014.pdf

### 05_NMR_simulation_machine_learning_matrix.pdf

- 内容：数值模拟：机器学习、神经网络、committee machine 与矩阵对角化方法
- 规模：10 个原始 PDF，153 页，估算 151,412 tokens。
- 包含文献/SI：
  - Asoodeh2015 NMRParametersDeterminationThro (26页；机器学习预测/参数估计)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Machine learning\Asoodeh2015_NMRParametersDeterminationThro.pdf
  - Simulation of NMR response from micro-CT images using artificial neural networks (8页；机器学习预测/参数估计；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Machine learning\Farzi2017_Simulation_artificial_neural_netw.pdf
  - Estimating NMR T2 distribution data from well log data with the use of a committee machine approach_ A case study from the Asmari formation in the Zagros Basin, Iran (14页；机器学习预测/参数估计)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Machine learning\Golsanami2014_CommitteeMachine.pdf
  - Type of the Paper (Article (27页；机器学习预测/参数估计)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Machine learning\Golsanami2021_NMRseismic.pdf
  - Neural network modeling of in situ fluid-filled pore size distributions in subsurface shale reservoirs under data constraints (13页；机器学习预测/参数估计；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Machine learning\Li2019_NeuralNetworkModelingOfInSituF.pdf
  - PII: S0920-4105(01)00089-4 (16页；机器学习预测/参数估计)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Machine learning\Mohaghegh2001_IntelligentSystemsReservoirCharacterization.pdf
  - Magnetization Evolution in Network Models of Porous Rock under Conditions of Drainage and Imbibition (12页；矩阵对角化/解析计算)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\matrix diagonalization methods\1-s2.0-S0021979702984729-main.pdf
  - Ioannidis.PDF (12页；矩阵对角化/解析计算)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\matrix diagonalization methods\Chang2000.pdf
  - 2001: Pore Network Simulation of Low-Field NMR Relaxometry Under Conditions of Drainage and Imbibition: Effects of Pore Structure and Saturation History (11页；矩阵对角化/解析计算)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\matrix diagonalization methods\Chang2001_drainage_conditions_saturation_history.pdf
  - Magnetization evolution in connected pore systems (14页；矩阵对角化/解析计算)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\matrix diagonalization methods\McCall1991.pdf

### 06_NMR_simulation_random_walk.pdf

- 内容：数值模拟：随机游走、扩散耦合、内部梯度、冻土/碳酸盐岩应用
- 规模：17 个原始 PDF，382 页，估算 248,132 tokens。
- 包含文献/SI：
  - Computational approach to integrate 3D X-ray microtomography and NMR data (9页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\1-s2.0-S109078071830123X-main.pdf
  - DF_Alhwety_v4_final_nodate (7页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Alhwety2014_Rock-typing_DiffCoupl.pdf
  - Carneiro2014 (8页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Carneiro2014.pdf
  - Diffusional coupling between microfractures and pore structure and its impact on nuclear magnetic resonance measurements in multiple-porosity systems (12页；随机游走模拟；扩散与弛豫机制；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Chi2015_DiffusionalCoupling.pdf
  - Fraga2013 RWCarbonatesPoreCoupling (4页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Fraga2013_RWCarbonatesPoreCoupling.pdf
  - Simulations of NMR Relaxation in a Real Porous Structure: Pre-asymptotic Behavior to the Localization Regime (15页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Gonzalez2020_Inhomogeneities .pdf
  - Guo et al. - 2016 - Numerical simulation of multi-dimensional NMR resp.pdf (10页；随机游走模拟；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Guo et al. - 2016 - Numerical simulation of multi-dimensional NMR resp.pdf
  - Imperial College London (163页；随机游走模拟；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\httpsimperialcollegelondon.box.comvportallive-51037696-pdf.pdf
  - Kaas2017 NMRforPermafrost (13页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Kaas2017_NMRforPermafrost.pdf
  - Leibig1993 RW (20页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Leibig1993_RW.pdf
  - Computational approach to integrate 3D X-ray microtomography and NMR data (9页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Lucas-Oliveira2018.pdf
  - Noetinger2016 preprint (45页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Noetinger2016_preprint.pdf
  - 2008: Pore-Scale Simulation of Nmr Response in Carbonates (12页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\SCA2008-30.pdf
  - Quantification of Multi-Phase Fluid Saturations in Complex Pore Geometries From Simulations of Nuclear Magnetic Resonance Measurements (13页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\toumelin2002.pdf
  - Toumelin2003 generalRW (11页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Toumelin2003_generalRW.pdf
  - Toumelin et al. - , C. Torres-Verdín.pdf (17页；随机游走模拟；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Toumelin2003_Temp&DiffusiveCoupling.pdf
  - doi:10.1016/j.jmr.2007.05.024 (14页；随机游走模拟)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR simulation\Random Walk\Toumelin2007_GeneralRW.pdf

### 07_NMR_theory_review_core.pdf

- 内容：理论与综述：NMR 原理、弛豫/扩散机制、近地表/油气应用综述
- 规模：13 个原始 PDF，241 页，估算 228,887 tokens。
- 包含文献/SI：
  - 2006 Yaramanci (21页；NMR Theory and Review)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\2006 Yaramanci.pdf
  - Behroozmand, Keating, Auken 2014 A Review of the Principles and Applications of the NMR Technique for Near Surface Characterization (59页；综述)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Behroozmand, Keating, Auken - 2014 - A Review of the Principles and Applications of the NMR Technique for Near-Surface Characterization.pdf
  - Importance of classical diffusion in NMR studies of water in biological cells (8页；扩散与弛豫机制)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\BrownsteinTarr1979.pdf
  - es3040686 1..6 (6页；NMR Theory and Review)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Environ. Sci. Technol 2013 Sanderlin.pdf
  - PII: 0022-2364(91)90213-D (14页；NMR Theory and Review)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Journal of Magnetic Resonance Series A 1991 Whittall.pdf
  - 2011-0462 365..377 (13页；NMR Theory and Review)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\keating2012.pdf
  - Mitchell (2012) In Situe Oil Monitoring Using NMR (24页；NMR Theory and Review；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Mitchell (2012) - In Situe Oil Monitoring Using NMR.pdf
  - Mohnke2015 triangular pore intro! (11页；NMR Theory and Review)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Mohnke2015_triangular_pore_intro!.pdf
  - Nuclear magnetic resonance average pore-size estimations outside the fast-diffusion regime (12页；扩散与弛豫机制；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Muller-Petke2015_DiffusionRegimes.pdf
  - Microsoft Word - diffusion.doc (11页；扩散与弛豫机制；可能为 SI/补充材料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\nmr_diffusion.pdf
  - Ramakrishnan1999 CarbonateRocks (11页；NMR Theory and Review)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Ramakrishnan1999_CarbonateRocks.pdf
  - A review on the applications of nuclear magnetic resonance (NMR) in the oil and gas industry: laboratory and field-scale measurements (38页；综述)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Review_Oil_Industry_2022.pdf
  - Magnetic Resonance of Porous Media (MRPM): A perspective (13页；NMR Theory and Review)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Song2012_NMR_PorousMedia_t2t2.pdf

### 08_NMR_theory_review_books_Coates_Dunn.pdf

- 内容：教材/专著类资料：Coates 与 Dunn 章节/材料
- 规模：14 个原始 PDF，543 页，估算 142,582 tokens。
- 包含文献/SI：
  - NMR Logging Principles and Applications (253页；NMR 测井/岩石物理教材资料)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Coates\1999 Coates.pdf
  - PII: S0950-1401(02)80012-X (3页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-1.pdf
  - PII: S0950-1401(02)80006-4 (28页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-10.pdf
  - PII: S0950-1401(02)80005-2 (30页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-11.pdf
  - PII: S0950-1401(02)80007-6 (57页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-12.pdf
  - PII: S0950-1401(02)80010-6 (49页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-13.pdf
  - PII: S0950-1401(02)80013-1 (15页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-3.pdf
  - PII: S0950-1401(02)80003-9 (2页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-4.pdf
  - PII: S0950-1401(02)80014-3 (7页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-5.pdf
  - PII: S0950-1401(02)80004-0 (11页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-6.pdf
  - PII: S0950-1401(02)80015-5 (11页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-7.pdf
  - PII: S0950-1401(02)80009-X (32页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-8.pdf
  - PII: S0950-1401(02)80008-8 (36页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn-9.pdf
  - PII: S0950-1401(02)80011-8 (9页；NMR 测井/岩石物理教材章节)
    - 原路径：C:\Users\imgw\Documents\Codex\gpt项目管理\NMR\原始文献布局\NMR Theory and Review\Dunn\2002 Dunn.pdf

## 重复与无效文件处理

- 可解析 PDF：95 个；按 SHA-256 去重后纳入合并：91 个。
- 完全重复副本：4 个，未重复合并，详见 `skipped_invalid_or_duplicate.csv`。
- 无法作为 PDF 打开的文件：23 个，多数为 `._*.pdf` 资源叉占位文件，未合并，详见 `skipped_invalid_or_duplicate.csv`。

## 配套文件

- `source_inventory.csv`：每篇纳入合并的源 PDF 清单、主题说明、页数、估算 token、来源路径。
- `GPT项目指令_NMR文献研究.md`：用于创建/配置 GPT 项目的项目指令。
