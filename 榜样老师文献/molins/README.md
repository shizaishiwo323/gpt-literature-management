# Molins 文献（孔隙尺度矿物溶解与反应输运）

Sergi Molins（Lawrence Berkeley National Laboratory）一组的五篇论文，按"论文名称 → 我的印象"整理。
用途：RTSPHEM 孔隙尺度方解石溶解模拟（level set + PHREEQC/SNIA 耦合）的对标与验证。

## 一览

| 文件（论文名称） | 年份 / 期刊 | 我的印象 | PDF |
|---|---|---|---|
| An investigation of the effect of pore scale flow on average geochemical reaction rates using direct numerical simulation | 2012, WRR | Molins 把孔隙尺度代码（Chombo）和真实化学反应库（CrunchFlow）耦合起来的奠基论文 | [PDF](./Water%20Resources%20Research%20-%202012%20-%20Molins%20-%20An%20investigation%20of%20the%20effect%20of%20pore%20scale%20flow%20on%20average%20geochemical.pdf) |
| Mineralogical and transport controls on the evolution of porous media texture using direct numerical simulation | 2017, WRR | 在 2012 代码基础上加入颗粒几何演化、用完整化学做的代码；我们正在复现的就是这篇 | [PDF](./Water%20Resources%20Research%20-%202017%20-%20Molins%20-%20Mineralogical%20and%20transport%20controls%20on%20the%20evolution%20of%20porous%20media%20texture.pdf) |
| Simulation of mineral dissolution at the pore scale with evolving fluid-solid interfaces: review of approaches and benchmark problem set | 2021, Comput. Geosci. | Molins 牵头的基准集合：多种方法 + 一阶线性反应速率 + 一个实验；我们的 TST 线性速率与它最对应 | [PDF](./Simulation%20of%20mineral%20dissolution%20at%20the%20pore%20scale%20with%20evolving%20fluid-solid%20interfaces%20review%20of%20approaches%20and%20benchmark%20problem%20set.pdf) |
| Determination of mineral dissolution regimes using flow-through time-resolved analysis (FT-TRA) and numerical simulation | 2016, Chem. Geol. | 实验论文：UBC 做单颗方解石流通实验，Molins 用他自己的孔隙尺度模型做三维模拟去拟合 | [PDF](./Determination%20of%20mineral%20dissolution%20regimes%20using%20flow-throughtime-resolved%20analysis%20%28FT-TRA%29%20and%20numerical%20simulation.pdf) |
| Pore-Scale Controls on Calcite Dissolution Rates from Flow-through Laboratory and Numerical Experiments | 2014, ES&T | Molins 通过一个实验去验证他们模型的准确性（注：实际结果是模型高估约 1.8 倍，文章用孔隙尺度模拟诊断偏差来源） | [PDF](./Pore-Scale%20Controls%20on%20Calcite%20Dissolution%20Rates%20from%20Flow-through%20Laboratory%20and%20Numerical%20Experiments.pdf) / [SI](./Pore-Scale%20Controls%20on%20Calcite%20Dissolution%20Rates%20from%20Flow-through%20Laboratory%20and%20Numerical%20Experiments%20-%20SI.pdf) |

## 逐篇说明

### 1. An investigation of the effect of pore scale flow on average geochemical reaction rates using direct numerical simulation

- 作者：Molins, Trebotich, Steefel, Shen
- 出处：Water Resources Research 48, W03527 (2012)，doi:10.1029/2011WR011404
- 文件：`Water Resources Research - 2012 - Molins - An investigation of the effect of pore scale flow on average geochemical.pdf`
- **我的印象**：Molins 耦合了真实化学反应库的代码，和 CrunchFlow 耦合（方法奠基篇）。
- 要点：
  - Chombo（不可压缩流 + 保守输运）+ CrunchFlow（多组分地球化学），SNIA 算子分裂耦合。
  - 完整碳酸盐化学；固体几何**不演化**。
  - 用单圆柱孔实验（Li et al. 2008）验证，用 1-D 连续尺度毛细管模型校核。
  - 结论：孔隙尺度流动不均匀会降低平均反应速率。

### 2. Mineralogical and transport controls on the evolution of porous media texture using direct numerical simulation

- 作者：Molins, Trebotich, Miller, Steefel
- 出处：Water Resources Research 53(5), 3645–3661 (2017)，doi:10.1002/2016WR020323
- 文件：`Water Resources Research - 2017 - Molins - Mineralogical and transport controls on the evolution of porous media texture.pdf`
- **我的印象**：Molins 耦合真实化学反应库（Chombo-Crunch，CrunchFlow）的代码，并加入了颗粒溶解的几何演化。
- 要点：
  - 嵌入边界 + level set 界面演化；完整碳酸盐化学；Chou et al. (1989) TST 速率律（k1、k2、k3 + 亲和项）。
  - 算例：单颗粒（0.0012–1.2 cm/s 四个流速）、双颗粒、颗粒堆、方解石–白云石裂隙。
  - 没有定量实验对比（裂隙算例仅与 Ellis et al. 2011 定性比较）。
  - RTSPHEM 当前在复现 §3.1 单颗粒 0.12 cm/s 算例（完整化学对标）。

### 3. Simulation of mineral dissolution at the pore scale with evolving fluid-solid interfaces: review of approaches and benchmark problem set

- 作者：Molins, Soulaine, Prasianakis, Abbasi, Poncet, Ladd, Starchenko, Roman, Trebotich, Tchelepi, Steefel
- 出处：Computational Geosciences 25, 1285–1318 (2021)，doi:10.1007/s10596-019-09903-x（开放获取）
- 文件：`Simulation of mineral dissolution at the pore scale with evolving fluid-solid interfaces review of approaches and benchmark problem set.pdf`
- **我的印象**：Molins 他们做的基准集合，里面有不同方法的线性（一阶）数值模拟和一个实验；我们目前做的 TST 线性反应速率和这个基准集合对应得比较好。
- 要点：
  - 5 个代码：Chombo-Crunch、OpenFOAM-DBS、格子 Boltzmann、Vortex、dissolFoam。
  - 化学刻意简化：CaCO3 + H+ → Ca2+ + HCO3-，r = k·a_H+，活度系数 1，只输运 H+；不含多组分化学。
  - Part I：二维单圆粒，固定几何；Part II：二维几何演化；Part III：三维实验验证（Soulaine et al. 2017 微流控方解石柱）。
  - 注意：是二维/三维，不是一维。RTSPHEM 已与 Part II 对标完成。

### 4. Determination of mineral dissolution regimes using flow-through time-resolved analysis (FT-TRA) and numerical simulation

- 作者：De Baere, Molins, Mayer, François
- 出处：Chemical Geology 430, 1–12 (2016)，doi:10.1016/j.chemgeo.2016.03.014
- 文件：`Determination of mineral dissolution regimes using flow-throughtime-resolved analysis (FT-TRA) and numerical simulation.pdf`
- **我的印象**：实验论文：UBC 做单颗方解石流通实验，Molins 用他自己的孔隙尺度模型做三维模拟去拟合。
- 要点：
  - FT-TRA 微型流通池（约 50 µL），ICP-MS 在线测出口 Ca；方解石单颗粒，pH 2.3 / 3.3 / 4.0，多个流量。
  - 三维模拟（直径 0.4 cm 圆柱 + 底部立方方解石颗粒，62.5 µm 分辨率），完整碳酸盐化学（EQ3/6 数据库）。
  - k1、k2 取自 Chou et al. (1989)，k3 = 2.34e-6 mol m⁻² s⁻¹ 取自 Busenberg & Plummer (1986)；不做标定即复现所有工况出口 Ca。
  - 可作为"完整化学 + 实验"的验证候选（需三维）。

### 5. Pore-Scale Controls on Calcite Dissolution Rates from Flow-through Laboratory and Numerical Experiments

- 作者：Molins, Trebotich, Yang, Ajo-Franklin, Ligocki, Shen, Steefel
- 出处：Environmental Science & Technology 48, 7453–7460 (2014)，doi:10.1021/es5013438
- 文件：`Pore-Scale Controls on Calcite Dissolution Rates from Flow-through Laboratory and Numerical Experiments.pdf`（正文）、`... - SI.pdf`（支持材料：控制方程、边界条件、化学体系与 logK）
- **我的印象**：Molins 通过一个实验去验证他们模型的准确性。
  - ⚠️ 补充更正：模型和实验**并不吻合**。孔隙尺度模拟和 1-D 连续模型的出口 Ca 都比实验高约 1.8–1.9 倍。文章的重点是把孔隙尺度模拟当作"数值实验"，拆分偏差来源：**输运限制**的贡献很小（约 5%），**速率律和参数**的贡献才是主要部分。
- 实验：
  - 熔融石英毛细管（内径 535 µm，装填长度 0.71235 cm），装填碎合成冰洲石（150–250 µm）。
  - 入口：0.01 M NaCl，与 4 bar pCO2 平衡（pH 3.609，Ca = 0）；流量 4.9 µL/min，持续 150 min，每 10 min 取样，用 ICP-MS 测 Ca。
  - 出口 Ca = 6.06 ± 0.34 mmol/L，达到稳态；平衡值为 16.67 mmol/L，说明体系远离平衡。只溶解了约 0.02% 的方解石，所以几何**不演化**。
- 模拟：
  - 孔隙尺度（Chombo-Crunch）：计算域由 XCMT 图像（体素 899 nm）重建，分辨率 2.32 µm，网格 3072×256×256（约 2 亿）；求解 NS + ADR，固液界面用嵌入边界；约 16 s 达到稳态，在 NERSC 上用 6144 核计算。
  - 连续尺度（CrunchFlow 1-D，160 个网格）：θ = 0.492，A = 20422 m²/m³ bulk（0.0148 m²/g，BET 测得 0.012 m²/g）；αL = 0.012 cm，由 Na 示踪剂标定；入口平均流速 0.0376 cm/s。
  - 化学体系：5 个主组分（H+, H2CO3*, Ca2+, Na+, Cl-）+ 9 个络合反应（logK 见 SI 表 3）。
  - TST 速率律：r = (k1·aH+ + k2·aH2CO3* + k3)(1 − 10^SI)，其中 k1 = 8e-6、k2 = 1.6e-8、k3 = 1.25e-9 **mol cm⁻² s⁻¹**（拟合 Pokrovsky et al. 2005/2009 转盘实验数据，425 rpm，25 °C；换算到 m⁻² 要 ×1e4）。
- 结果（出口 Ca，mmol/L）：实验 6.06 ± 0.34；孔隙尺度 10.91；连续尺度 11.55；平衡值 16.67。
  - 输运控制：入口附近颗粒周围有扩散边界层（宽 30–55 µm，pH 3.6–3.8 → 4.2–4.5）；小孔隙只靠扩散交换物质，处于近平衡状态；Na 穿透曲线呈非 Fick 型拖尾。
  - 表面控制：只标定 k3（k1 = k2 = 0）去拟合实验，得到的速率明显低于 Pokrovsky 的数据（Fig. 6）。可能原因：样品不同、TST 形式本身的局限、扩散中没有考虑电化学效应。
- 对 RTSPHEM 的意义：
  - 这是"完整化学 + 三维实验 + 固定几何"的案例，可以单独检验反应–输运耦合，不涉及 level set。
  - 计算域依赖 XCMT 图像，网格量大约 2 亿，完整复现很难。较现实的做法是复现 1-D 连续模型的 11.55 mmol/L，用来检查化学体系和速率参数有没有设对。
  - 对标时应以**模拟值**为准：原文模型本身就和实验差约 1.8 倍，不能拿实验值当真值。

## 验证链（RTSPHEM）

| 层级 | 论文 | 化学 | 对比对象 |
|---|---|---|---|
| 1 | Molins 2021 Part II | 简化一阶 | 5 个代码 |
| 2 | Molins 2017 §3.1 | 完整 + 数据库 | Chombo-Crunch 数值解 |
| 3a | Molins 2021 Part III | 简化一阶 | 三维实验 |
| 3b | De Baere 2016 | 完整 + 数据库 | 三维实验出口 Ca |
| 3c | Molins 2014 ES&T | 完整 + 数据库（几何不演化） | 1-D 连续模型 11.55 mmol/L / 孔隙尺度 10.91 mmol/L（实验 6.06，原文模型本身高估约 1.8 倍） |
