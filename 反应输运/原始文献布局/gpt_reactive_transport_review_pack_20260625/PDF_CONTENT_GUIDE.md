# 反应输运复现文献包说明
本目录把三个来源目录中的 41 个 PDF 整合为 7 个专题 PDF，便于放入 GPT 项目作为论文分析、代码审阅和 PHREEQC 耦合反应输运复现的本地知识库。原始 PDF 未移动、未删除、未覆盖。
## 合并结果
| 编号 | 合并 PDF | 主题 | 原始 PDF 数 | 页数 | 估算 tokens | 低于 200 万 tokens |
|---|---|---|---:|---:|---:|---|
| 01 | `merged_pdfs/01_chombo_crunch_molins_core_methods.pdf` | Chombo-Crunch / Molins pore-scale reactive transport core methods | 7 | 138 | 165980 | 是 |
| 02 | `merged_pdfs/02_deng_fracture_dissolution_2013_2020.pdf` | Deng fracture dissolution and carbonate alteration, 2013-2020 | 9 | 163 | 195600 | 是 |
| 03 | `merged_pdfs/03_pore_fracture_precipitation_and_dissolution_2018_2020.pdf` | Pore/fracture precipitation and dissolution mechanisms, 2018-2020 | 7 | 128 | 153600 | 是 |
| 04 | `merged_pdfs/04_precipitation_and_coupled_fracture_processes_2021_2022.pdf` | Precipitation and coupled fracture processes, 2021-2022 | 4 | 63 | 75600 | 是 |
| 05 | `merged_pdfs/05_recent_weathering_co2_texture_and_upscaling_2023_2024.pdf` | Recent weathering, CO2 storage, texture, and upscaling, 2023-2024 | 6 | 78 | 99004 | 是 |
| 06 | `merged_pdfs/06_recent_shale_dissolution_precipitation_reviews_2025_2026.pdf` | Recent shale, two-phase dissolution, and precipitation reviews, 2025-2026 | 5 | 86 | 107914 | 是 |
| 07 | `merged_pdfs/07_caco3_precipitation_benchmark_yoon_zhang_si.pdf` | CaCO3 precipitation benchmark: Zhang experiment, Yoon simulation, and SI | 3 | 23 | 28376 | 是 |

## 每个合并 PDF 的内容

### 01 - Chombo-Crunch / Molins pore-scale reactive transport core methods
- 文件：`merged_pdfs/01_chombo_crunch_molins_core_methods.pdf`
- 内容：Chombo-Crunch, embedded-boundary flow/transport, pore-scale dissolution benchmarks, and Molins/Trebotich/Steefel direct numerical simulation papers.
- 规模：7 个源 PDF，138 页，估算 165980 tokens。
- 包含论文/SI：
  - `Water Resources Research - 2012 - Molins - An investigation of the effect of pore scale flow on average geochemical.pdf`（11 页）：Uses direct numerical simulation to show how pore-scale flow and transport limitations affect average geochemical reaction rates; important for separating intrinsic PHREEQC kinetics from transport-limited apparent rates.
  - `Trebotich et al. 2014 — High-resolution simulation of pore-scale reactive transport processes associated with carbon sequestration.pdf`（10 页）：Introduces Chombo-Crunch as a high-resolution image-based pore-scale reactive transport capability for CO2-related fluid-rock systems.
  - `Molins et al. 2014 — Pore-scale controls on calcite dissolution rates from flow-through laboratory and numerical experiments.pdf`（8 页）：Combines flow-through calcite experiments, xCT geometry, and pore-scale simulation to diagnose calcite dissolution rate controls and model-experiment mismatch.
  - `Trebotich & Graves 2015 — An adaptive finite volume method for the incompressible Navier–Stokes equations in complex geometries.pdf`（44 页）：Numerical-method foundation for embedded-boundary/adaptive finite-volume Navier-Stokes flow in complex pore/fracture geometries.
  - `Water Resources Research - 2017 - Molins - Mineralogical and transport controls on the evolution of porous media texture.pdf`（17 页）：Explores how mineralogical heterogeneity and transport limitations drive texture evolution during dissolution/precipitation in direct numerical simulations.
  - `Simulation of mineral dissolution at the pore scale with evolving fluid-solid interfaces_ review of approaches and benchmark problem set.pdf`（34 页）：Review and benchmark suite comparing pore-scale dissolution/interface-evolution codes, including Chombo-Crunch, useful for validation targets.
  - `Trebotich et al. 2024 — A multiphysics coupling framework for exascale simulation of fracture evolution in subsurface energy applications.pdf`（14 页）：Modern coupling-framework paper for multiphysics fracture evolution, useful for thinking about modular coupling and exascale solver organization.

### 02 - Deng fracture dissolution and carbonate alteration, 2013-2020
- 文件：`merged_pdfs/02_deng_fracture_dissolution_2013_2020.pdf`
- 内容：Deng-led carbonate fracture alteration, xCT/TILT image processing, 2.5D fracture reactive transport, multimineral fracture evolution, and acid erosion.
- 规模：9 个源 PDF，163 页，估算 195600 tokens。
- 包含论文/SI：
  - `2013_Modifications_Carbonate_Fracture_Hydrodynamic_Properties.pdf`（42 页）：Deng et al. study of CO2-acidified brine altering carbonate fracture hydrodynamic properties from xCT-derived aperture and flow analysis.
  - `2015_Alterations_fractures_carbonate_CO2_brines.pdf`（9 页）：High-pressure CO2-brine fracture alteration experiments showing geometry and hydrodynamic changes under different CO2 conditions; includes supporting information marker.
  - `2016_TILT_Fracture_Geometry_Xray_Tomography.pdf`（14 页）：TILT segmentation method for x-ray tomography of fractures; directly relevant to converting images into apertures/geometries for simulations.
  - `2016_2_5D_Reactive_Transport_Model.pdf`（9 页）：Deng/Molins/Steefel 2.5D fracture alteration model; key paper for learning the reduced-dimensional fracture reactive-transport coupling strategy.
  - `2017_Alteration_Erosion_Carbonate_Rich_Shale_Fracture.pdf`（25 页）：Reactive transport model for carbonate-rich shale fracture alteration and erosion; emphasizes fracture-matrix reactions and synchrotron observations.
  - `2018_Fracture_Evolution_Multimineral_Systems.pdf`（28 页）：Analyzes how mineral composition, flow rate, and aperture heterogeneity control fracture evolution in multimineral systems.
  - `2018_Planar_fractures_limestone_flow_heterogeneity.pdf`（15 页）：Examines planar limestone fracture evolution under flow/mineral heterogeneity and local transport processes; useful for aperture-permeability coupling logic.
  - `2019_Fracture_Channelization_Transmissivity_Evolution.pdf`（12 页）：Focuses on channelization and transmissivity evolution in dissolving fractures, a key behavior to reproduce or test against.
  - `2020_Acid_erosion_carbonate_fractures_arsenic.pdf`（9 页）：Connects acid erosion of carbonate fractures with arsenic release/transport, highlighting reactive alteration plus contaminant consequences.

### 03 - Pore/fracture precipitation and dissolution mechanisms, 2018-2020
- 文件：`merged_pdfs/03_pore_fracture_precipitation_and_dissolution_2018_2020.pdf`
- 内容：Surface roughness, fracture reactive transport modeling, multiscale fractured media, hydrodynamic dissolution in cavities, MRI/SEM barite precipitation, nanoparticle transport, and rough-fracture dissolution models.
- 规模：7 个源 PDF，128 页，估算 153600 tokens。
- 包含论文/SI：
  - `2018_Pore_scale_surface_roughness_reaction_rates.pdf`（16 页）：Studies how pore-scale surface roughness influences reaction rates and apparent kinetics.
  - `2019_Modeling_reactive_transport_fractures.pdf`（26 页）：Concise modeling-oriented fracture reactive transport paper, useful for equations, assumptions, and coupling choices.
  - `2019_Multiscale_reactive_transport_fractured_media.pdf`（21 页）：Multiscale treatment of reactive transport in fractured media; useful for linking pore/fracture-scale models to continuum descriptions.
  - `2020_Hydrodynamic_driven_dissolution_embedded_cavities.pdf`（17 页）：Hydrodynamically driven dissolution in embedded cavities; useful for understanding local flow focusing and dissolution morphology.
  - `2020_MRI_SEM_barite_precipitation.pdf`（20 页）：Uses MRI/SEM to characterize barite precipitation and pore/fracture changes, relevant to precipitation validation data.
  - `2020_Nanoparticle_transport_low_field_NMR.pdf`（9 页）：Nanoparticle transport study using low-field NMR; less central to PHREEQC coupling but useful for NMR-aware porous-media diagnostics.
  - `2020_Semi_analytical_mineral_dissolution_rough_fractures.pdf`（19 页）：Semi-analytical dissolution model for rough fractures; useful as a lower-complexity check against numerical simulations.

### 04 - Precipitation and coupled fracture processes, 2021-2022
- 文件：`merged_pdfs/04_precipitation_and_coupled_fracture_processes_2021_2022.pdf`
- 内容：Barite scale deposition, pore-scale precipitation effects on diffusivity, coupled fracture-matrix alteration, and two-phase flow controls on mineral reaction rates.
- 规模：4 个源 PDF，63 页，估算 75600 tokens。
- 包含论文/SI：
  - `2021_Barite_scale_deposition_Marcellus_shale.pdf`（11 页）：Barite scale deposition in shale context; relevant to precipitation clogging and permeability change mechanisms.
  - `2021_Pore_scale_precipitation_diffusivity.pdf`（17 页）：Pore-scale precipitation effects on diffusivity; useful for coupling mineral volume change to transport-property updates.
  - `2022_Coupled_processes_fractures_bordering_matrix.pdf`（18 页）：Coupled fracture and adjacent matrix processes; useful for handling reactive fronts, altered layers, and matrix exchange.
  - `2022_Two_phase_flow_mineral_reaction_rates.pdf`（17 页）：Two-phase flow controls on mineral reaction rates; useful if later extending PHREEQC coupling beyond single-phase flow.

### 05 - Recent weathering, CO2 storage, texture, and upscaling, 2023-2024
- 文件：`merged_pdfs/05_recent_weathering_co2_texture_and_upscaling_2023_2024.pdf`
- 内容：Enhanced rock weathering, dissolution-regime scaling, CO2 storage coupling, micro-porosity/mineralogical texture, and permeability-porosity upscaling under precipitation.
- 规模：6 个源 PDF，78 页，估算 99004 tokens。
- 包含论文/SI：
  - `2023_environmental_controls_enhanced_rock_weathering.pdf`（10 页）：Enhanced rock weathering efficiency and environmental controls; broader reactive-transport context for weathering simulations.
  - `2023_environmental_controls_enhanced_rock_weathering_repository.pdf`（11 页）：Repository/manuscript copy of the enhanced rock weathering work; kept with the main paper because it may contain provenance or alternative formatting.
  - `2023_Surface_volume_scaling_dissolution_regimes.pdf`（11 页）：Surface-volume scaling controlled by dissolution regimes; useful for dimensional analysis and upscaling dissolution rates.
  - `2024_Fluid_dynamics_geochemistry_CO2_storage_perspective.pdf`（18 页）：Perspective/review on fluid dynamics and geochemistry coupling in CO2 storage, reactive transport modeling, and upscaling.
  - `2024_Micro_porosity_mineralogical_texture_fractured_rock.pdf`（14 页）：Effects of micro-porosity and mineralogical texture on fractured-rock alteration; useful for heterogeneous matrix/fracture models.
  - `2024_mineral_precipitation_geometry_alteration.pdf`（14 页）：Pore-scale precipitation and permeability-porosity relationship upscaling under geometry alteration.

### 06 - Recent shale, two-phase dissolution, and precipitation reviews, 2025-2026
- 文件：`merged_pdfs/06_recent_shale_dissolution_precipitation_reviews_2025_2026.pdf`
- 内容：Shale stimulation geochemistry, intragranular porosity effects, barite precipitation under nucleation/advection controls, two-phase hydrodynamic dissolution, and a 2026 precipitation review.
- 规模：5 个源 PDF，86 页，估算 107914 tokens。
- 包含论文/SI：
  - `2025_acid_spearhead_slickwater_wolfcamp_shale.pdf`（24 页）：Geochemical impact of acid spearhead/slickwater stimulation on Wolfcamp shale; application case for reactive fracture-rock alteration.
  - `2025_Intragranular_porosity_mineral_dissolution_rates.pdf`（17 页）：Micro-continuum treatment of well-connected intragranular porosity and its impact on mineral dissolution rates.
  - `2025_Nucleation_advection_barite_precipitation.pdf`（10 页）：Microfluidic study of nucleation and advection controls on barite precipitation in fractured porous media.
  - `2026_Dissolution_rates_two_phase_hydrodynamics_single_pores.pdf`（12 页）：Benchmark-like single-pore two-phase calcite dissolution simulations and scaling laws.
  - `2026_Mineral_precipitation_porous_media_systems.pdf`（23 页）：Review of mineral precipitation in porous media, covering nucleation, growth, pore-size/substrate controls, and porous-media evolution.

### 07 - CaCO3 precipitation benchmark: Zhang experiment, Yoon simulation, and SI
- 文件：`merged_pdfs/07_caco3_precipitation_benchmark_yoon_zhang_si.pdf`
- 内容：Transverse-mixing-induced CaCO3 precipitation in a micromodel, pore-scale simulation benchmark, and the supporting information figures.
- 规模：3 个源 PDF，23 页，估算 28376 tokens。
- 包含论文/SI：
  - `pore-scale-study-of-transverse-mixing-induced-caco3-precipitation-and-permeability-reduction-in-a-model-subsurface.pdf`（6 页）：Experimental micromodel paper on transverse-mixing-induced CaCO3 precipitation and permeability reduction; benchmark target for simulation reproduction.
  - `es1019788_si_001.pdf`（6 页）：Supporting information for the Zhang et al. CaCO3 precipitation micromodel paper, including supplementary figures and imaging details.
  - `Water Resources Research - 2012 - Yoon - Pore‐scale simulation of mixing‐induced calcium carbonate precipitation and.pdf`（11 页）：Pore-scale simulation of mixing-induced CaCO3 precipitation/dissolution in a microfluidic pore network; natural template for PHREEQC-coupled reproduction.

## 建议阅读顺序
1. 先读 `01_chombo_crunch_molins_core_methods.pdf`，建立 Chombo-Crunch/Molins 的孔尺度耦合、嵌入边界、界面演化和 benchmark 概念。
2. 再读 `02_deng_fracture_dissolution_2013_2020.pdf`，抓住 Deng 系列从实验/xCT 到 2.5D fracture RTM 的建模路线。
3. 读 `07_caco3_precipitation_benchmark_yoon_zhang_si.pdf`，把 CaCO3 沉淀 benchmark、实验观测、Yoon 模拟和 SI 参数对齐。
4. 用 `03`、`04`、`05`、`06` 补充沉淀、粗糙裂隙、两相流、孔隙结构、upscaling 和近期综述。

## 用于代码审阅的关注点
- PHREEQC 耦合：化学状态变量、反应步长、传输步长、operator splitting/迭代耦合是否清楚。
- 几何演化：矿物体积分数、孔隙/固体界面、aperture 或 porosity 更新是否守恒且可追踪。
- 参数复现：是否记录 Da、Pe、流速、初始/边界浓度、反应速率常数、矿物表面积、时间步和单位。
- 验证：是否能复现论文的浓度突破曲线、沉淀形态、孔隙率/渗透率变化或 benchmark 图。
