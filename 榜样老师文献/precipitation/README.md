# precipitation 文献（孔隙尺度混合诱导碳酸钙沉淀与溶解）

Hongkyu Yoon（Sandia National Laboratories）与 Valocchi、Werth（UIUC）、Dewers 合作的孔隙尺度 CaCO3 沉淀/溶解模拟论文，按"论文名称 → 我的印象"整理。

**我的印象**：结构非常严谨、论证非常详实的碳酸钙沉淀模拟文献。可以作为三方面的强参考文献：
1. **写作引用**的强参考文献；
2. **复现**的强参考文献；
3. **学习论文写作**的强参考文献。

## 一览

| 文件（论文名称） | 年份 / 期刊 | 我的印象 | PDF |
|---|---|---|---|
| Pore-scale simulation of mixing-induced calcium carbonate precipitation and dissolution in a microfluidic pore network | 2012, WRR | 结构严谨、论证详实的 CaCO3 沉淀模拟；写作引用、复现、学习写作三方面的强参考 | [PDF](./Water%20Resources%20Research%20-%202012%20-%20Yoon%20-%20Pore-scale%20simulation%20of%20mixing-induced%20calcium%20carbonate%20precipitation%20and.pdf) |

## 逐篇说明

### 1. Pore-scale simulation of mixing-induced calcium carbonate precipitation and dissolution in a microfluidic pore network

- 作者：Hongkyu Yoon, Albert J. Valocchi, Charles J. Werth, Thomas Dewers
- 出处：Water Resources Research 48, W02524 (2012)，doi:10.1029/2011WR011192
- 文件：`Water Resources Research - 2012 - Yoon - Pore-scale simulation of mixing-induced calcium carbonate precipitation and.pdf`
- 支持材料（SI）：原文没有 SI 或辅助材料，正文已给出全部方程（式 1–13）、参数（Table 1）和工况（Table 2）。
- 被引：Crossref 154 次，Semantic Scholar 153 次（2026-11 查询）。
- **我的印象**：结构非常严谨、论证非常详实的碳酸钙沉淀模拟文献；可作为写作引用、复现、学习论文写作的强参考文献。
- 要点：
  - 对标实验：Zhang et al. (2010, ES&T, doi:10.1021/es1019788) 的微模型横向混合实验。1 cm × 2 cm，圆柱直径 300 µm，孔体 180 µm，孔喉 40 µm，深 20 µm，孔隙度约 0.39；达西速度 1.25 cm/min；CaCl2 与 Na2CO3 各 25 mM（0.025 mol/L）。只模拟靠近入口的前三个孔体。
  - 核心现象：沉淀面积约 13 min 内快速上升，随后快速下降，3–4 h 后到达较低平台（作者称 overshoot）。
  - 二维化依据：深度方向扩散时间约 0.1 s（L²/D，L 取半深 10 µm），远小于停留时间约 2 min（Pe 约 100）。
  - 模型三模块：LBM（BGK，反弹无滑移）稳态 Stokes 流；FVM 多组分反应输运（SIA-1，所有物种同一 D = 9.0e-10 m²/s）；固相更新（V_m 显式更新）。
  - 化学：主物种 Ca2+、H+、CO3 2-，次级物种 OH-、HCO3-、H2CO3(aq)；扩展 Debye-Hückel 活度；只考虑球霰石（K_sp = 1.832e-2 mol² m⁻⁶，摩尔体积 3.747e-5 m³/mol）。
  - 速率律：Chou et al. (1989)，I_m = −(k1·aH+ + k2·aH2CO3 + k3)(1 − Ω)，k1 = 8.9e-1、k2 = 5.01e-4、k3 = 6.6e-7 mol m⁻² s⁻¹。均相反应按瞬时平衡，非均相反应作为反应面边界条件（式 2）。
  - 关键设定：
    - 反应表面积 = 网格上下板面积（dz = 20 µm）+ 相邻圆柱壁面；这是复现初期快速沉淀的必要条件。
    - 流动（堵塞）阈值 V_m,TV = 0.6（0.5–0.75 不敏感）；沉淀计数阈值 V_m > 0.05（只用于后处理统计面积）。
    - 有效扩散 D_eff = D(1 − V_m)^n（Archie 型），n 默认 2。
    - 溶解因子 d_f：只乘在溶解上，集总参数，分不清是速率常数还是表面积变大。
  - 网格：5 µm（一个颗粒 60 格，孔喉 7 格）；1 µm 加密对比沉淀质量差 < 3%。
  - 五个工况（Table 2）：case 1 基准；case 2/3 为 n = 0/3；case 4 为 k_cc × 2；case 5 为 d_f = 300。
  - 结果：
    - 基准工况复现了沉淀形态、早期速率和最大沉淀面积，但溶解太慢。
    - 改 n、改 k_cc 都复现不了 13 min 后的下降；k_cc × 2 反而因提前堵塞使最大沉淀量下降。
    - d_f = 300 可匹配到约 30 min；之后中心线上方 pH 和 Ω 偏高，溶解仍偏慢。
  - 作者承认的局限：加速溶解的机理不清楚；推测是纳米蚀坑、纳米颗粒使表面积增大，以及重结晶（球霰石 → 方解石、Ostwald 熟化），但没有直接证据。
- 作为三类参考的用法：
  - **写作引用**：孔隙尺度矿物沉淀/溶解建模、混合诱导沉淀、沉淀对扩散和流动的反馈、反应表面积不确定性。
  - **复现**：代码未开源（作者自编 LB-FVM），但方程、参数、几何、工况都在正文中给全，可据此重写；或用 PHREEQC（KINETICS/RATES）+ 自编输运代码重建。注意 d_f 的物理意义不唯一，复现时建议把沉淀和溶解速率分开写、考虑球霰石/方解石两相。
  - **学习写作**：
    - 引言四步走：背景 → 批次实验多、输运条件少 → 模型缺少与实验的定量对比 → 本文三个目标。
    - 方法逐条列出假设，每个参数都给出取值依据或标定范围。
    - 结果按"一个候选原因一个小节"组织（4.2 扩散、4.3 速率常数、4.4 溶解因子），先排除再确认。
    - 结论如实区分"已解释"和"未解释"，主动承认局限并给出文献支撑的推测。

## 相关文献（未放 PDF）

| 论文 | 出处 | 说明 |
|---|---|---|
| Zhang et al., Pore-scale study of transverse mixing induced CaCO3 precipitation and permeability reduction in a model subsurface sedimentary system | ES&T 44(20), 7833–7838 (2010)，doi:10.1021/es1019788 | 本文对标的实验；Crossref 被引 161 次 |
| Yoon, Kang & Valocchi, Lattice Boltzmann-based approaches for pore-scale reactive transport | Rev. Mineral. Geochem. 80, 393–431 (2015) | 同一团队的 LBM 反应输运综述，重写代码时可参考 |
