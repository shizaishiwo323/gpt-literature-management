# precipitation 文献（孔隙尺度混合诱导碳酸钙沉淀与溶解）

Werth（UIUC）、Valocchi 团队及其合作者（PNNL 的 Zhang 等，Sandia 的 Yoon 等）关于孔隙尺度混合诱导 CaCO3 沉淀/溶解的实验和模拟论文，按"论文名称 → 我的印象"整理。两篇是一组：Zhang et al. (2010) 是微流控实验，Yoon et al. (2012) 是对标这组实验的孔隙尺度模拟。

## 一览

| 文件（论文名称） | 年份 / 期刊 | 我的印象 | PDF | SI |
|---|---|---|---|---|
| Pore-scale study of transverse mixing induced CaCO3 precipitation and permeability reduction in a model subsurface sedimentary system | 2010, ES&T | 微流控 CaCO3 沉淀实验的早期研究；有三维形貌表征方法（激光共聚焦）；可作为微流控实验来源的参考 | [PDF](./Environmental%20Science%20and%20Technology%20-%202010%20-%20Zhang%20-%20Pore-scale%20study%20of%20transverse%20mixing%20induced%20CaCO3%20precipitation%20and%20permeability%20reduction.pdf) | [SI](./SI%20-%20Environmental%20Science%20and%20Technology%20-%202010%20-%20Zhang%20-%20Pore-scale%20study%20of%20transverse%20mixing%20induced%20CaCO3%20precipitation%20and%20permeability%20reduction.pdf) |
| Pore-scale simulation of mixing-induced calcium carbonate precipitation and dissolution in a microfluidic pore network | 2012, WRR | 结构严谨、论证详实的 CaCO3 沉淀模拟；写作引用、复现、学习写作三方面的强参考 | [PDF](./Water%20Resources%20Research%20-%202012%20-%20Yoon%20-%20Pore-scale%20simulation%20of%20mixing-induced%20calcium%20carbonate%20precipitation%20and.pdf) | 无 |

## 逐篇说明

### 1. Pore-scale study of transverse mixing induced CaCO3 precipitation and permeability reduction in a model subsurface sedimentary system

- 作者：Changyong Zhang, Karl Dehoff, Nancy Hess, Mart Oostrom, Thomas W. Wietsma, Albert J. Valocchi, Bruce W. Fouke, Charles J. Werth
- 出处：Environmental Science & Technology 44(20), 7833–7838 (2010)，doi:10.1021/es1019788
- 文件：`Environmental Science and Technology - 2010 - Zhang - Pore-scale study of transverse mixing induced CaCO3 precipitation and permeability reduction.pdf`
- 支持材料（SI）：`SI - Environmental Science and Technology - 2010 - Zhang - ....pdf`，共 6 页 5 张图，都是图件，没有数据表：
  - Fig. S1：0.65 µm 高分辨率图像，用于晶型（形貌）判别；
  - Fig. S2：中间两个饱和度（Ωc/Ωv = 3.8/3.1、4.6/3.9）整体沉淀像素数随时间变化；
  - Fig. S3：同两个饱和度下上游、中游、下游单孔的沉淀曲线；
  - Fig. S4：单孔 CaCO3 沉淀的 3D 激光共聚焦图像（3.4/2.8、4.6/3.9）和不同深度的 2D 共聚焦切片；
  - Fig. S5：沉淀前后荧光示踪剂分布（4 个饱和度），图中可直接看到柱子的交错排布。
- 被引：Crossref 161 次（2026-11 查询）。
- 数据公开情况：没有数据可用性声明，原始图像（每个时间点 25 × 3 = 75 张分幅图）、阈值和曲线数值都没有公开；需要数据只能从 Fig. 4、5、S2、S3 数字化，或联系通讯作者 Werth。
- **我的印象**：
  1. 做**微流控碳酸钙沉淀实验的早期研究**；
  2. 有**三维形貌**的表征方法（Leica SP2 激光共聚焦，面内 0.21 µm、层厚 0.5 µm，荧光素充满孔隙后成像）；
  3. 可以作为**微流控实验来源**的参考（微模型设计、制作与实验流程）。
- 要点：
  - 微模型：硅片刻蚀（光刻 + ICP-DRIE），1100 °C 氧化 1 h（氧化层约 0.1 µm），阳极键合 Pyrex 盖片；孔隙网络 2 cm × 1 cm，圆柱直径 300 µm，孔体 180 µm，孔喉 40 µm，深 17–21 µm，孔隙度 0.39；柱子交错排布。
  - 实验：CaCl2 与 Na2CO3 等摩尔 6.5、10、25、50 mM 四组（Table 1，Ω 实为 log 值：Ωc/Ωv = 3.4/2.8、3.8/3.1、4.6/3.9、5.2/4.5）；A、B 两入口等流量，达西速度 1.25 cm/min（ISCO 100DM）；入口 C 注 HCl（pH 1.5–2.0，流量为总流量一半）防止出口堵塞；每组两次平行。
  - 表征：Nikon Eclipse 2000 TE 反射 DIC 显微成像 + 拼图 + 阈值统计沉淀像素；拉曼背散射（514 nm）鉴定晶型；荧光示踪（示踪剂:水 = 2:1）判断渗透率变化；激光共聚焦看 3D 形貌。
  - 结果：
    - 饱和度越高，沉淀带越窄（约 2 个孔体 → <1 个孔体）、初始速率越大（3.1×10⁴ → 4.0×10⁵ pixel/h）、沉淀总量越少（最低饱和度约为最高的 5 倍）。
    - 只有球霰石和方解石，没有文石；球霰石占比 80% → >95%。
    - 高饱和度下入口附近早期沉淀会再溶解（Fig. 6）。
    - 沉淀占满约 20 µm 全深度；示踪剂横向占比从 2/3 降到 1/2，说明中线沉淀带堵塞孔隙、阻断横向混合。
  - 作者承认的局限：渗透率没有直接测量，只是定性评估；像素数只是表观速率（沉淀密度不均、未必占满深度）；体系只含 Ca²⁺/CO₃²⁻，二维均质，不代表真实储层条件。
- 作为参考的用法：
  - **实验来源**：微模型几何、制作工艺、流速和浓度设计可直接引用；Yoon et al. (2012) 的模拟就是对标这组实验（25 mM 工况）。
  - **三维形貌方法**：共聚焦 + 荧光素充填判断沉淀是否占满深度、孔隙是否被堵死。
  - **写作引用**：混合诱导沉淀的自我限制（沉淀阻断混合）、饱和度对晶型和沉淀量的影响、羽流边缘沉淀对 CO2 封存注入能力的影响。

### 2. Pore-scale simulation of mixing-induced calcium carbonate precipitation and dissolution in a microfluidic pore network

- 作者：Hongkyu Yoon, Albert J. Valocchi, Charles J. Werth, Thomas Dewers
- 出处：Water Resources Research 48, W02524 (2012)，doi:10.1029/2011WR011192
- 文件：`Water Resources Research - 2012 - Yoon - Pore-scale simulation of mixing-induced calcium carbonate precipitation and.pdf`
- 支持材料（SI）：原文没有 SI 或辅助材料，正文已给出全部方程（式 1–13）、参数（Table 1）和工况（Table 2）。
- 被引：Crossref 154 次，Semantic Scholar 153 次（2026-11 查询）。
- **我的印象**：结构非常严谨、论证非常详实的碳酸钙沉淀模拟文献；可作为写作引用、复现、学习论文写作的强参考文献。
- 要点：
  - 对标实验：Zhang et al. (2010, ES&T, doi:10.1021/es1019788) 的微模型横向混合实验（即本目录第 1 篇）。1 cm × 2 cm，圆柱直径 300 µm，孔体 180 µm，孔喉 40 µm，深 20 µm，孔隙度约 0.39；达西速度 1.25 cm/min；CaCl2 与 Na2CO3 各 25 mM（0.025 mol/L）。只模拟靠近入口的前三个孔体。
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
| Yoon, Kang & Valocchi, Lattice Boltzmann-based approaches for pore-scale reactive transport | Rev. Mineral. Geochem. 80, 393–431 (2015) | 同一团队的 LBM 反应输运综述，重写代码时可参考 |
