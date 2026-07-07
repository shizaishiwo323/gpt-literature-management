# GPT 文献包内容说明

生成时间：2026-07-03 14:08:11

本目录把指定路径中的 PDF 按内容哈希去重后整合为 8 个主题 PDF。原始完整页面被保留；合并 PDF 内为每篇来源 PDF 添加了书签。

## 合并 PDF 总览

| 合并 PDF | 内容 | 来源 PDF 数 | 页数 | 估算 tokens | 大小 |
| --- | --- | ---: | ---: | ---: | ---: |
| `01_foundational_theory_schakel_pride_liu.pdf` | 经典理论基础：Pride 耦合方程、Schakel/Smeulders 流体-多孔介质界面边界条件、Liu 有限偏移距 VSEP 谱积分、电震/震电基本波动性质。 | 7 | 73 | 81056 | 4.88 MB |
| `02_recent_seismoelectric_experiments_models.pdf` | 近期震电实验与数值模拟：有限偏移距、界面全波形、电导率/饱和度/孔渗影响、水槽和现场/实验验证、谱比方法。 | 16 | 368 | 300911 | 53.5 MB |
| `03_reactive_transport_prior_work_and_si.pdf` | 反应输运与已有研究材料：孔隙尺度溶蚀、虫洞化、方解石反应输运自电位，以及当前项目已有 manuscript 和 supporting information。 | 5 | 119 | 89227 | 20.54 MB |
| `04_literature_review_core_bridge.pdf` | 综述桥接与跨主题核心文献：用于把震电、反应输运、孔隙演化、Pride 理论和论文引言/讨论连接起来的核心材料。 | 1 | 19 | 17100 | 2.66 MB |
| `05_conductivity_electrolyte_streaming_zeta.pdf` | 电解质、电导率、pH、温盐与 streaming/zeta potential：支撑流体电导率、H+ 浓度和界面电动耦合参数映射。 | 7 | 174 | 112584 | 12.48 MB |
| `06_revil_applications_inversion_unsaturated.pdf` | Revil 系列应用、反演与非饱和/多相震电研究：油水界面、交叉孔成像、虚电极、联合反演、波束形成等应用背景。 | 11 | 201 | 170216 | 41.55 MB |
| `07_seismoelectric_books_reviews.pdf` | 震电方法书籍与长综述：Revil 方法书、Grobbe 震电勘探书籍/章节、Jouniaux-Zyserman 综述等高层框架。 | 3 | 813 | 721384 | 113.65 MB |
| `08_calcite_zeta_carbonate_reference.pdf` | 方解石/碳酸盐 zeta potential 与电导率参考：用于约束碳酸盐溶蚀体系中的表面电性、CO2 影响和天然石灰岩参数。 | 3 | 86 | 65079 | 11.22 MB |

## 每个合并 PDF 包含的文献

### 01_foundational_theory_schakel_pride_liu.pdf
经典理论基础：Pride 耦合方程、Schakel/Smeulders 流体-多孔介质界面边界条件、Liu 有限偏移距 VSEP 谱积分、电震/震电基本波动性质。

1. Seismoelectric reflection and transmission at a fluid porous-medium interface (9 页，估算 12962 tokens)
   - 内容用途：与震电、反应输运或电动参数有关的补充文献，适合在写作时按具体问题检索引用。
   - 来源：`uploaded_files\01_classical_theory_foundational_papers\01-Seismoelectric reflection and transmission at a fluid_porous-medium interface.pdf`
2. Schakel 2011 JAP laboratory theory (5 页，估算 5782 tokens)
   - 内容用途：Schakel/Smeulders 界面理论与边界条件来源，适合核对反射/透射转换系数和相位约定。
   - 来源：`uploaded_files\01_classical_theory_foundational_papers\02_Schakel_2011_JAP_laboratory_theory.pdf`
3. Liu 2018 finite offset VSEP (7 页，估算 6196 tokens；另有 1 个重复来源已去重)
   - 内容用途：有限偏移距 VSEP 和 interface EM 波形建模参考，适合核对频率-波数积分、空间分布和偶极子解释。
   - 来源：`uploaded_files\01_classical_theory_foundational_papers\03_Liu_2018_finite_offset_VSEP.pdf`
4. Schakel 2011 Geophysics interface forward model (8 页，估算 7712 tokens)
   - 内容用途：Schakel/Smeulders 界面理论与边界条件来源，适合核对反射/透射转换系数和相位约定。
   - 来源：`uploaded_files\01_classical_theory_foundational_papers\04_Schakel_2011_Geophysics_interface_forward_model.pdf`
5. Electroseismic wave properties (15 页，估算 17040 tokens)
   - 内容用途：与震电、反应输运或电动参数有关的补充文献，适合在写作时按具体问题检索引用。
   - 来源：`uploaded_files\01_classical_theory_foundational_papers\Electroseismic wave properties.pdf`
6. Governing equations for the coupled electromagnetics and acoustics of porous media (19 页，估算 17825 tokens)
   - 内容用途：Pride 震电耦合控制方程基础，适合定义动态渗透率、电动耦合和电磁-声学耦合框架。
   - 来源：`uploaded_files\01_classical_theory_foundational_papers\Governing equations for the coupled electromagnetics and acoustics of porous media.pdf`
7. Electroseismic Wave Theory of Frenkel and More Recent Developments (10 页，估算 13539 tokens)
   - 内容用途：Pride 震电耦合控制方程基础，适合定义动态渗透率、电动耦合和电磁-声学耦合框架。
   - 来源：`uploaded_files\01_classical_theory_foundational_papers\pride2005.pdf`

### 02_recent_seismoelectric_experiments_models.pdf
近期震电实验与数值模拟：有限偏移距、界面全波形、电导率/饱和度/孔渗影响、水槽和现场/实验验证、谱比方法。

1. The effect of layer thickness and fluid conductivity contrasts on seismoelectric signals : insights from laboratory experiments and numerical simulations (20 页，估算 24567 tokens；另有 1 个重复来源已去重)
   - 内容用途：电导率、盐度、pH 或电解质影响参考，适合把 H+ 浓度/流体电导率映射到震电参数。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\01_Martins-Gomes_2026_layer_thickness_conductivity.pdf`
2. Conductivity dependence of seismoelectric wave phenomena in fluidsaturated sediments (12 页，估算 14887 tokens；另有 1 个重复来源已去重)
   - 内容用途：电导率、盐度、pH 或电解质影响参考，适合把 H+ 浓度/流体电导率映射到震电参数。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\02_Block_Harris_2006_conductivity_dependence.pdf`
3. The effect of rock permeability and porosity on seismoelectric conversion: experiment and analytical modelling (34 页，估算 20669 tokens；另有 1 个重复来源已去重)
   - 内容用途：孔隙率/渗透率对震电转换的影响参考，适合支持水文参数敏感性分析。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\03_Peng_2019_permeability_porosity.pdf`
4. Seismoelectric wave conversions at an interface: a quantitative comparison between laboratory data and full-waveform modelling (21 页，估算 23373 tokens)
   - 内容用途：与震电、反应输运或电动参数有关的补充文献，适合在写作时按具体问题检索引用。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\04_Martins-Gomes_2023_interface_full_waveform.pdf`
5. Experimental quantification of the seismoelectric transfer function and its dependence on conductivity and saturation in loose sand (33 页，估算 28200 tokens)
   - 内容用途：电导率、盐度、pH 或电解质影响参考，适合把 H+ 浓度/流体电导率映射到震电参数。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\07_Holzhauer_2017_conductivity_saturation_loose_sand.pdf`
6. Zhu Toksoz 1996 author technical report (30 页，估算 8204 tokens)
   - 内容用途：与震电、反应输运或电动参数有关的补充文献，适合在写作时按具体问题检索引用。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\09a_Zhu_Toksoz_1996_author_technical_report.pdf`
7. Zhu et al 1997 author technical report (22 页，估算 6653 tokens)
   - 内容用途：与震电、反应输运或电动参数有关的补充文献，适合在写作时按具体问题检索引用。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\09b_Zhu_et_al_1997_author_technical_report.pdf`
8. Water Table and Permeability Estimation From Multi‐Channel Seismoelectric Spectral Ratios (29 页，估算 29981 tokens)
   - 内容用途：与震电、反应输运或电动参数有关的补充文献，适合在写作时按具体问题检索引用。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\10_Hu_2023_JGR_spectral_ratios.pdf`
9. Schakel 2012 fluid porous interface (12 页，估算 8795 tokens；另有 1 个重复来源已去重)
   - 内容用途：Schakel/Smeulders 界面理论与边界条件来源，适合核对反射/透射转换系数和相位约定。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\12_Schakel_2012_fluid_porous_interface.pdf`
10. Microsoft Word - zhu_revised.doc (25 页，估算 9452 tokens)
   - 内容用途：与震电、反应输运或电动参数有关的补充文献，适合在写作时按具体问题检索引用。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\18_Zhu_Burns_Toksoz_2008_water_tank.pdf`
11. Wapenaar 2012 experimental validation interferometry (24 页，估算 25225 tokens)
   - 内容用途：实验验证或水槽研究，适合对照模型波形、界面响应和观测可行性。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\22_Wapenaar_2012_experimental_validation_interferometry.pdf`
12. jb008053 1..15 (15 页，估算 13273 tokens)
   - 内容用途：与震电、反应输运或电动参数有关的补充文献，适合在写作时按具体问题检索引用。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\23_Tardif_2011_frequency_dependent_Ottawa_sand.pdf`
13. Experimental Measurement of Frequency-Dependent Permeability and Streaming Potential of Sandstones (29 页，估算 18297 tokens)
   - 内容用途：震电/电震综述，适合写引言、应用背景、机制分类和研究空缺。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\25_Jouniaux_2020_frequency_dependent_permeability_streaming.pdf`
14. Full waveform numerical simulations of seismoelectromagnetic wave conversions in fluid‐saturated stratified porous media (19 页，估算 19671 tokens)
   - 内容用途：与震电、反应输运或电动参数有关的补充文献，适合在写作时按具体问题检索引用。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\27_Garambois_Dietrich_2002_full_waveform.pdf`
15. Jouniaux Zyserman 2016 seismoelectric review (36 页，估算 43690 tokens；另有 2 个重复来源已去重)
   - 内容用途：震电/电震综述，适合写引言、应用背景、机制分类和研究空缺。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\31_Jouniaux_Zyserman_2016_seismoelectric_review.pdf`
16. Seismoelectric interface electromagnetic wave characteristics for the finite offset Vertical Seismoelectric Profiling configuration Theoretical modeling and experiment verification (7 页，估算 5974 tokens)
   - 内容用途：有限偏移距 VSEP 和 interface EM 波形建模参考，适合核对频率-波数积分、空间分布和偶极子解释。
   - 来源：`uploaded_files\02_recent_seismoelectric_research_experiments_simulations\Seismoelectric interface electromagnetic wave characteristics for the finite offset Vertical Seismoelectric Profiling configuration_ Theoretical modeling and experiment verification.pdf`

### 03_reactive_transport_prior_work_and_si.pdf
反应输运与已有研究材料：孔隙尺度溶蚀、虫洞化、方解石反应输运自电位，以及当前项目已有 manuscript 和 supporting information。

1. Interpreting Self-Potential Signal during Reactive Transport: Application to Calcite Dissolution and Precipitation (31 页，估算 23416 tokens；另有 1 个重复来源已去重)
   - 内容用途：方解石/碳酸盐表面电性与 zeta potential 参考，适合约束溶蚀体系界面电动参数。
   - 来源：`uploaded_files\03_previous_reactive_transport_research\29_Rembert_2022_calcite_reactive_transport_SP.pdf`
2. Soulaine 2017 pore scale dissolution wormholing (27 页，估算 20908 tokens；另有 1 个重复来源已去重)
   - 内容用途：孔隙尺度反应输运、矿物溶蚀或孔隙合并参考，适合连接孔渗/曲折度演化与震电响应。
   - 来源：`uploaded_files\03_previous_reactive_transport_research\30_Soulaine_2017_pore_scale_dissolution_wormholing.pdf`
3. manuscript (18 页，估算 15756 tokens)
   - 内容用途：当前项目已有反应输运-NMR 主文稿，可用于对接本项目论文背景、数据来源和多物理耦合叙事。
   - 来源：`uploaded_files\03_previous_reactive_transport_research\manuscript.pdf`
4. supporting information (27 页，估算 7842 tokens)
   - 内容用途：当前项目已有补充信息，包含方法细节、补充图表或参数信息，需与主文稿一起引用。
   - 来源：`uploaded_files\03_previous_reactive_transport_research\supporting information.pdf`
5. Pore-merging methodology for reactive transport and mineral dissolution in pore-network models (16 页，估算 21305 tokens)
   - 内容用途：孔隙尺度反应输运、矿物溶蚀或孔隙合并参考，适合连接孔渗/曲折度演化与震电响应。
   - 来源：`uploaded_files\literature_review\Pore_merging_reactive_transport_mineral_dissolution_2021.pdf`

### 04_literature_review_core_bridge.pdf
综述桥接与跨主题核心文献：用于把震电、反应输运、孔隙演化、Pride 理论和论文引言/讨论连接起来的核心材料。

1. Pride 1994 governing equations (19 页，估算 17100 tokens)
   - 内容用途：Pride 震电耦合控制方程基础，适合定义动态渗透率、电动耦合和电磁-声学耦合框架。
   - 来源：`uploaded_files\literature_review\Pride_1994_governing_equations.pdf`

### 05_conductivity_electrolyte_streaming_zeta.pdf
电解质、电导率、pH、温盐与 streaming/zeta potential：支撑流体电导率、H+ 浓度和界面电动耦合参数映射。

1. Frequency-Dependent Streaming Potentials (10 页，估算 9948 tokens)
   - 内容用途：震电/电震综述，适合写引言、应用背景、机制分类和研究空缺。
   - 来源：`uploaded_files\literature_review\conductivity_electrolyte_seismoelectric\2001_Reppert_Morgan_Lesmes_Jouniaux_frequency_dependent_streaming_potentials.pdf`
2. Zhu Toksoz effects saturant conductivity seismoelectric conversion (8 页，估算 11819 tokens)
   - 内容用途：电导率、盐度、pH 或电解质影响参考，适合把 H+ 浓度/流体电导率映射到震电参数。
   - 来源：`uploaded_files\literature_review\conductivity_electrolyte_seismoelectric\2003_Zhu_Toksoz_effects_saturant_conductivity_seismoelectric_conversion.pdf`
3. IFP whitepaper seismo electromagnetic method (14 页，估算 7639 tokens)
   - 内容用途：电导率、盐度、pH 或电解质影响参考，适合把 H+ 浓度/流体电导率映射到震电参数。
   - 来源：`uploaded_files\literature_review\conductivity_electrolyte_seismoelectric\2016_IFP_whitepaper_seismo_electromagnetic_method.pdf`
4. Modelling pH-Dependent and Microstructure-Dependent Streaming Potential Coefficient and Zeta Potential of Porous Sandstones (26 页，估算 16562 tokens)
   - 内容用途：电导率、盐度、pH 或电解质影响参考，适合把 H+ 浓度/流体电导率映射到震电参数。
   - 来源：`uploaded_files\literature_review\conductivity_electrolyte_seismoelectric\2018_Glover_Walker_modelling_pH_microstructure_streaming_zeta_potentials.pdf`
5. Measurements of the Relationship Between Microstructure, pH, and the Streaming and Zeta Potentials of Sandstones (24 页，估算 16177 tokens)
   - 内容用途：电导率、盐度、pH 或电解质影响参考，适合把 H+ 浓度/流体电导率映射到震电参数。
   - 来源：`uploaded_files\literature_review\conductivity_electrolyte_seismoelectric\2018_Walker_Glover_microstructure_pH_streaming_zeta_potentials_sandstones.pdf`
6. Seismo-electric conversion in shale: experiment and analytical modelling (44 页，估算 25009 tokens)
   - 内容用途：电导率、盐度、pH 或电解质影响参考，适合把 H+ 浓度/流体电导率映射到震电参数。
   - 来源：`uploaded_files\literature_review\conductivity_electrolyte_seismoelectric\2020_Peng_Di_Glover_seismo_electric_conversion_shale.pdf`
7. Modified theoretical model for temperature-dependent electro-kinetic properties of porous media (48 页，估算 25430 tokens)
   - 内容用途：电导率、盐度、pH 或电解质影响参考，适合把 H+ 浓度/流体电导率映射到震电参数。
   - 来源：`uploaded_files\literature_review\conductivity_electrolyte_seismoelectric\2026_Glover_temperature_salinity_pH_electrokinetic_properties_porous_media_AAM.pdf`

### 06_revil_applications_inversion_unsaturated.pdf
Revil 系列应用、反演与非饱和/多相震电研究：油水界面、交叉孔成像、虚电极、联合反演、波束形成等应用背景。

1. Revil Linde Cerepi electrokinetic coupling unsaturated porous media (45 页，估算 14816 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2007_Revil_Linde_Cerepi_electrokinetic_coupling_unsaturated_porous_media.pdf`
2. Stochastic joint inversion of 2D seismic and seismoelectric signals in linear poroelastic materials: A numerical investigation (13 页，估算 19521 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2010_Jardani_Revil_Slob_Sollner_stochastic_joint_inversion_Geophysics.pdf`
3. gji_4439_LR (17 页，估算 18686 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2010_Revil_Jardani_seismoelectric_response_heavy_oil_reservoirs.pdf`
4. Imaging with crosshole seismoelectric tomography (18 页，估算 17448 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2012_Araji_Revil_Jardani_Minsley_crosshole_seismoelectric_tomography_GJI.pdf`
5. Virtual electrode current injection using seismic focusing and seismoelectric conversion (5 页，估算 6099 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2012_Sava_Revil_virtual_electrode_current_injection.pdf`
6. Seismoelectric conversion generated from water-oil boundary in unsaturated porous media (6 页，估算 5081 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2013_Mahardika_Revil_water_oil_boundary_SEG.pdf`
7. Coupled hydromechanical and electromagnetic disturbances in unsaturated porous materials (23 页，估算 23963 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2013_Revil_Mahardika_coupled_hydromechanical_electromagnetic_unsaturated.pdf`
8. Revil Barnier Karaoulis Sava unsaturated porous media (18 页，估算 17870 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2014_Revil_Barnier_Karaoulis_Sava_unsaturated_porous_media.pdf`
9. Sava Revil Karaoulis crosswell resistivity seismoelectric focusing (15 页，估算 13541 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2014_Sava_Revil_Karaoulis_crosswell_resistivity_seismoelectric_focusing.pdf`
10. ElKhoury Revil Sava seismoelectric beamforming sensitivity (20 页，估算 15243 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2015_ElKhoury_Revil_Sava_seismoelectric_beamforming_sensitivity.pdf`
11. Jardani Revil two immiscible fluid phases (21 页，估算 17948 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2015_Jardani_Revil_two_immiscible_fluid_phases.pdf`

### 07_seismoelectric_books_reviews.pdf
震电方法书籍与长综述：Revil 方法书、Grobbe 震电勘探书籍/章节、Jouniaux-Zyserman 综述等高层框架。

1. The SeismoelectricMethodTheory and applications revil (298 页，估算 219316 tokens；另有 2 个重复来源已去重)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\01_classical_theory_foundational_papers\The SeismoelectricMethodTheory and applications revil.pdf`
2. Grobbe et al Seismoelectric Exploration chp1-2 (43 页，估算 40034 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2020_Grobbe_et_al_Seismoelectric_Exploration_chp1-2.pdf`
3. Grobbe et al Seismoelectric Exploration full book (472 页，估算 462034 tokens)
   - 内容用途：Revil 系列理论、应用或反演研究，适合支撑震电应用背景、非饱和/多相效应和成像解释。
   - 来源：`uploaded_files\literature_review\revil_seismoelectric\2020_Grobbe_et_al_Seismoelectric_Exploration_full_book.pdf`

### 08_calcite_zeta_carbonate_reference.pdf
方解石/碳酸盐 zeta potential 与电导率参考：用于约束碳酸盐溶蚀体系中的表面电性、CO2 影响和天然石灰岩参数。

1. Influence of CO2 on the Electrical Conductivity and Streaming Potential of Carbonate Rocks (18 页，估算 18190 tokens)
   - 内容用途：电导率、盐度、pH 或电解质影响参考，适合把 H+ 浓度/流体电导率映射到震电参数。
   - 来源：`uploaded_files\zeta-calcite\JGR Solid Earth - 2019 - Cherubini - Influence of CO2 on the Electrical Conductivity and Streaming Potential of Carbonate.pdf`
2. Zeta potential of artificial and natural calcite in aqueous solution (17 页，估算 26731 tokens)
   - 内容用途：方解石/碳酸盐表面电性与 zeta potential 参考，适合约束溶蚀体系界面电动参数。
   - 来源：`uploaded_files\zeta-calcite\Zeta potential of artifi cial and natural calcite in aqueous solution.pdf`
3. Zeta Potential of Intact Natural Limestone (51 页，估算 20158 tokens)
   - 内容用途：方解石/碳酸盐表面电性与 zeta potential 参考，适合约束溶蚀体系界面电动参数。
   - 来源：`uploaded_files\zeta-calcite\Zeta Potential of Intact Natural Limestone.pdf`

## 去重说明
相同哈希的 PDF 只合并一次；全部来源路径保存在 `source_manifest.csv` 的 `all_sources` 字段。
