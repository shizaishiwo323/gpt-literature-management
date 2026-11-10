# zhangchi 文献（SIP 不同极化机制的孔隙尺度模拟与 NMR-SIP 联合反演）

Chi Zhang（两篇论文署名单位均为 The University of Kansas, Department of Geology）与 Qifei Niu 合作的两篇论文，按"论文名称 → 我的印象"整理。

**两篇共同的印象**：文章写作非常好，非常便于阅读理解，章节结构、逻辑、故事性都安排得非常好。

## 一览

| 文件（论文名称） | 年份 / 期刊 | 我的印象 | PDF |
|---|---|---|---|
| Joint inversion of NMR and SIP data to estimate pore size distribution of geomaterials | 2018, Geophys. J. Int. | 做 NMR-SIP 的联合反演；文章写作非常好，非常便于阅读理解 | [PDF](./Joint%20inversion%20of%20NMR%20and%20SIP%20data%20to%20estimate%20pore%20size%20distribution%20of%20geomaterials.pdf) |
| A Framework for Pore-Scale Simulation of Effective Electrical Conductivity and Permittivity of Porous Media in the Frequency Range From 1 mHz to 1 GHz | 2020, JGR: Solid Earth | 做 SIP 不同机制的模拟；文章写作非常好，非常便于阅读理解 | [PDF](./A%20Framework%20for%20Pore-Scale%20Simulation%20of%20Effective%20Electrical%20Conductivity%20and%20Permittivity%20of%20Porous%20Media%20in%20the%20Frequency%20Range%20From%201%20mHz%20to%201%20GHz.pdf) |

## 逐篇说明

### 1. Joint inversion of NMR and SIP data to estimate pore size distribution of geomaterials

- 作者：Qifei Niu, Chi Zhang
- 出处：Geophysical Journal International 212, 1791–1805 (2018)，doi:10.1093/gji/ggx501
- 文件：`Joint inversion of NMR and SIP data to estimate pore size distribution of geomaterials.pdf`
- **我的印象**：做 NMR-SIP 的联合反演。文章写作非常好，非常便于阅读理解，章节结构、逻辑、故事性都安排得非常好。
- 要点：
  - 思路：NMR T2 弛豫和低频 SIP 都受孔隙几何控制，二者通过各自的岩石物理模型与孔径 r 相联系；表面性质相近时，SIP 弛豫时间 τ 正比于 T2 的平方（文中用 Osterman et al. 2016 的 Sherwood 砂岩数据检验）。
  - 方法：岩石物理联合反演，写成非线性最小二乘问题；Tikhonov 正则约束孔径分布的光滑性，两步法确定两组数据的权衡和数据拟合与正则的平衡；Gauss–Newton 迭代求解，灵敏度矩阵解析计算。
  - 合成样品：双峰孔径分布（两个对数正态，平均孔径 20 µm 和 2 µm，权重 0.4 和 0.6）。Case 1 用准确的岩石物理模型；Case 2 用简化（不准确）的模型，仍能恢复孔径分布的主要特征。
  - 相比单独反演，加入另一组数据能提高孔径分布的分辨率；已知双电层离子扩散系数时，联合反演还能估计表面弛豫率。
  - Berea 砂岩应用：孔隙度 20.2%，地层因子 16.3，NaCl 溶液 0.043 S/m；NMR 为 2 MHz CPMG（回波间隔 100 µs），SIP 频率范围 10⁻³ Hz–10 kHz；反演得到的孔径分布与压汞结果较为一致。

### 2. A Framework for Pore-Scale Simulation of Effective Electrical Conductivity and Permittivity of Porous Media in the Frequency Range From 1 mHz to 1 GHz

- 作者：Qifei Niu, Chi Zhang, Manika Prasad
- 出处：Journal of Geophysical Research: Solid Earth 125, e2020JB020515 (2020)，doi:10.1029/2020JB020515
- 文件：`A Framework for Pore-Scale Simulation of Effective Electrical Conductivity and Permittivity of Porous Media in the Frequency Range From 1 mHz to 1 GHz.pdf`
- **我的印象**：做 SIP 不同机制的模拟。文章写作非常好，非常便于阅读理解，章节结构、逻辑、故事性都安排得非常好。
- 要点：
  - 框架三步：从二值微观结构图像求几何性质（孔隙度、比表面积、孔径分布、孔喉长度分布，用孔隙网络提取算法）→ 计算电化学极化引起的复电导 → 用动态孔径 Λ 升尺度，Δσ*_w = 2C*/Λ，作为水相额外的复电导率。
  - 同时考虑界面极化（电学不连续引起）和电化学极化：孔隙节点上的孔隙极化（Schwarz 1962 模型，将颗粒尺寸换成孔径）、孔喉上的膜极化（Titov et al. 2002 窄孔喉模型）。
  - Berea 砂岩验证：μCT 二值图像 350³ 体素，分辨率 2.8 µm，孔隙度 20.2%，地层因子 16.3，NaCl 溶液 0.043 S/m；模拟频率 10⁻³–10⁹ Hz，与实验的有效电导率和介电常数谱总体吻合良好。
  - 单独模拟每种极化的贡献：高频（>10⁵ Hz）界面极化主导；中频（10²–10⁵ Hz）膜极化贡献显著，忽略它会使模拟的有效介电常数远小于实测；低于 100 Hz 孔隙极化占主导。
  - 文中讨论的差异：界面极化的特征频率模拟低于实验（约 5×10⁵ Hz 对约 10⁷ Hz），可解释为图像的固液界面比真实样品光滑；低频（<0.1 Hz）模拟的介电常数系统性偏低，可能因为模拟体积小（约 1 mm³），未包含更大孔隙的极化。
  - 数据：http://doi.org/10.5281/zenodo.3908737（论文 Data Availability Statement 给出）。
