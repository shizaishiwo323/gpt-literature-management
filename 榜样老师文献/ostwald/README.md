# ostwald 文献（Ostwald ripening：孔隙网络 / 气泡熟化 + 沉淀 / 相场）

2026-11-18 从 `shizaishiwo323/RTSPHEM-main` 的 `literature/` 整体迁移过来（原样保留两个子目录、PDF 和 `notes/` 文本），目的是减轻 RTSPHEM-main 的体量。

**作者核查结论**：这里不全是 Martin J. Blunt 的文章。真正有 Blunt 署名的只有 4 篇（下表标 ★）；`11_Blunt_2022_...` 虽然文件名带 Blunt，但文件本身是下载失败的 HTML 页面，不是 PDF。

**注意**：标"⚠ HTML"的文件扩展名是 `.pdf`，实际是网页/错误页（下载失败），需要重新下载；标"⚠ 空"的文件只有空白内容。

## ostwald_ripening_pnm/（多孔介质中气泡 Ostwald ripening、孔隙网络模型）

| 文件 | 作者（第一页核对） | 状态 |
|---|---|---|
| 01_Adebimpe_2026_Time_dependent_PNM_Ostwald_ripening.pdf | Adebimpe, Foroughi, Bijeljic, **Blunt** ★ | arXiv 2605.10955 |
| 02_Adebimpe_2024_Percolation_without_trapping_PRE.pdf | Adebimpe, Foroughi, Bijeljic, **Blunt** ★ | arXiv 2404.01313 |
| 03_Laku_2026_Modeling_Ostwald_Ripening_Dynamics_iPNM.pdf | Laku, Salehpour, Lan, Zhao, Mehmani | arXiv 2604.06581 |
| 04_Salehpour_2025_Ostwald_Ripening_Underground_Gas_Storage.pdf | Salehpour, Lan, Bueno, Laku, Mehmani, Zhao | arXiv 2509.00044 |
| 05_deChalendar_2018_Pore_scale_modelling_Ostwald_ripening_JFM.pdf | de Chalendar, Garing, Benson | JFM 835 |
| 06_Singh_2022_Level_set_approach_Ostwald_ripening_TIPM.pdf | — | ⚠ HTML |
| 07_Xu_2017_Egalitarianism_among_bubbles_PRL.pdf | — | ⚠ HTML |
| 08_Xu_2019_Gravity_induced_bubble_ripening_GRL.pdf | — | ⚠ 空 |
| 09_Yu_2023_Bubble_Coarsening_Kinetics_GRL.pdf | Yu, Wang, Liu, Mao, Mehmani, Xu | GRL 2023 |
| 10_Wang_2021_Capillary_equilibrium_bubbles_PNAS.pdf | — | ⚠ HTML |
| 11_Blunt_2022_Ostwald_ripening_gravitational_equilibrium_PRE.pdf | （应为 Blunt 2022 PRE） | ⚠ HTML |
| 12_Li_2021_Long_Term_Redistribution_Residual_Gas_TIPM.pdf | Li, Orr, Benson | TIPM 141 |
| 13_Goodarzi_2024_Trapping_hysteresis_Ostwald_hydrogen_IJHE.pdf | Goodarzi, Zhang, Foroughi, Bijeljic, **Blunt** ★ | IJHE 56 |
| 14_Zhang_2023_Pore_scale_observations_H2_trapping_GRL.pdf | Zhang, …, **Blunt** ★（通讯作者） | GRL 2023 |
| 15_Bueno_2024_Generalized_kinetic_theory_Ostwald_porous_media_poster.pdf | Bueno, Ayala, Mehmani | 海报 |
| 16_Li_2020_Diffusion_induced_gas_redistribution_slides.pdf | Li, Benson | 报告幻灯片 |
| 17_Li_2020_Continuum_scale_representation_Ostwald_JFM.pdf | Li, Garing, Benson | JFM 889 |
| 18_Bueno_2026_Kinetic_theory_multicomponent_Ostwald_arxiv.pdf | Bueno, Ayala, Mehmani | arXiv 2512.20665 |

`notes/Blunt_2026_source.txt` 是 01 号文章（Adebimpe et al. 2026）的全文文本；`notes/pdf_text/` 是各 PDF 的抽取文本。

## ostwald_ripening_precipitation/（矿物沉淀、相场 / 经典 Ostwald ripening 理论、反应输运）

| 文件 | 作者（第一页核对） | 状态 |
|---|---|---|
| 01_Fan_2002_..._high_volume_fraction.pdf | — | ⚠ HTML |
| 01_Fan_2002_..._alt_http.pdf | Fan, Chen, Chen, Voorhees | Acta Mater. 50 |
| 02_Yao_1993_Theory_and_simulation_of_Ostwald_ripening.pdf | Yao 等（扫描版，无文字层） | PDF |
| 03_PRISMS_PF_DeWitt_2020_..._framework.pdf | — | ⚠ HTML |
| 03_PRISMS_PF_DeWitt_2020_..._framework_alt.pdf | DeWitt, Rudraraju, Montiel, Andrews, Thornton | npj Comput. Mater. 6 |
| 04_FiPy_Guyer_2009_....pdf | Guyer, Wheeler, Warren | CiSE 2009 |
| 05_MOOSE_MARMOT_Schwen_2017_....pdf | Schwen, Aagesen, Peterson, Tonks | INL 接收稿 |
| 06_Deng_2021_WRR_....pdf | Deng, Tournassat, Molins, Claret, Steefel | WRR 2021 |
| 07_Ling_2024_WRR_....pdf | **实际作者**：Wang, Hu, Steefel（文件名中 "Ling" 与内容不符） | WRR 60(6) |
| 08_Steefel_Maher_2009_....pdf | Steefel, Maher | RiMG 70 |
| 09_Steefel_Hu_2022_....pdf | **实际作者**：Seigneur, Mayer 等（RiMG 85, 2019；文件名与内容不符） | RiMG 85 |
| 11_Calcite_precipitation_in_porous_media_XMT_modeling.pdf | Noiriel 等，Chem. Geol. 2012 | PDF |
| 12_Van_Westen_2018_temperature_cycling_Ostwald_ripening.pdf | — | ⚠ 空 |
| 14_TEN_2024_advective_Cahn_Hilliard_....pdf | ten Eikelder, Khanwale | CTR Summer Program 2024 |
| 15_Voorhees_1985_Theory_of_Ostwald_ripening.pdf / _alt | — | ⚠ HTML（两个都是） |
| 16_Ratke_Voorhees_..._book.pdf / _alt | — | ⚠ HTML（两个都是） |
| 18_Iggland_Mazzotti_2012_....pdf | — | ⚠ HTML |
| 19_Vetter_2013_....pdf | — | ⚠ HTML |
| 20_Moats_2019_....pdf | — | ⚠ HTML |
| 21_Yoon_2012_WRR_CaCO3_microfluidic_pore_network.pdf | — | ⚠ HTML |
