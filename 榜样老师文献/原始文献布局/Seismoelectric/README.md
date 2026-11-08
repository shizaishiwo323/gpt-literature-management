# Seismoelectric 文献（震电效应：理论基石、实验与数值模拟复现）

震电效应相关的 5 篇论文，按"论文名称 → 我的印象"整理。
主线：Pride 理论（基石） → Schakel & Smeulders 界面反射/透射公式 → Schakel 2011 实验 + 模拟 → 刘老师（Yukai Liu）VSEP 数值模拟与实验（复现来源）。

## 一览

| 文件（论文名称） | 年份 / 期刊 | 我的印象 |
|---|---|---|
| Governing equations for the coupled electromagnetics and acoustics of porous media | 1994, Phys. Rev. B | 震电效应中 Pride 理论的基石论文 |
| Electroseismic wave properties | 1996, JASA | 震电效应中 Pride 理论的基石论文 |
| Seismoelectric reflection and transmission at a fluid/porous-medium interface | 2010, JASA | 刘老师数值模拟所使用的理论公式的来源 |
| Laboratory measurements and theoretical modeling of seismoelectric interface response and coseismic wave fields | 2011, J. Appl. Phys. | Schakel 2011 实验和模拟的论文，适合做基石 |
| Seismoelectric interface electromagnetic wave characteristics for the finite offset Vertical Seismoelectric Profiling configuration: Theoretical modeling and experiment verification | 2018, JASA | 刘老师的数值模拟工作和实验工作，是我复现的来源 |

## 逐篇说明

### 1. Governing equations for the coupled electromagnetics and acoustics of porous media

- 作者：Steven R. Pride
- 出处：Physical Review B 50(21), 15678–15696 (1994)，doi:10.1103/PhysRevB.50.15678
- 文件：`Governing equations for the coupled electromagnetics and acoustics of porous media.pdf`
- **我的印象**：震电效应中 Pride 理论的基石论文。
- 要点：从第一性原理推导流体饱和多孔介质中电磁场与声学（Biot 波）耦合的宏观控制方程（Pride 方程）。

### 2. Electroseismic wave properties

- 作者：Steven R. Pride, Matthijs W. Haartsen
- 出处：J. Acoust. Soc. Am. 100(3), 1301–1315 (1996)，doi:10.1121/1.416018
- 文件：`Electroseismic wave properties.pdf`
- **我的印象**：震电效应中 Pride 理论的基石论文。
- 要点：在 Pride (1994) 方程基础上给出震电波的一般性质，为求解震电边值问题提供理论背景。

### 3. Seismoelectric reflection and transmission at a fluid/porous-medium interface

- 作者：Menne D. Schakel, David M. J. Smeulders（TU Delft）
- 出处：J. Acoust. Soc. Am. 127(1), 13–21 (2010)，doi:10.1121/1.3263613
- 文件：`Seismoelectric reflection and transmission at a fluid_porous-medium interface.pdf`
- **我的印象**：这篇论文主要是刘老师数值模拟使用的理论公式的来源。
- 要点：用包含黏性与电动耦合的等效密度表述震电波频散关系，推导流体/多孔介质界面的电动反射与透射系数。

### 4. Laboratory measurements and theoretical modeling of seismoelectric interface response and coseismic wave fields

- 作者：M. D. Schakel, D. M. J. Smeulders, E. C. Slob, H. K. J. Heller
- 出处：Journal of Applied Physics 109, 074903 (2011)，doi:10.1063/1.3567945
- 文件：`Laboratory measurements and theoretical modeling of seismoelectric interface response and coseismic wave fields.pdf`
- **我的印象**：Schakel 2011 实验和模拟的论文，适合做基石。
- 要点：实验室测量震电界面响应和同震波场，并与理论模拟对比，可作为数值复现的实验—模拟对标基准。

### 5. Seismoelectric interface electromagnetic wave characteristics for the finite offset Vertical Seismoelectric Profiling configuration: Theoretical modeling and experiment verification

- 作者：Yukai Liu（刘老师）, David Smeulders, Yuanda Su, Xiaoming Tang
- 出处：J. Acoust. Soc. Am. 143, EL13 (2018)，doi:10.1121/1.5020261
- 文件：`Seismoelectric interface electromagnetic wave characteristics for the finite offset Vertical Seismoelectric Profiling configuration_ Theoretical modeling and experiment verification.pdf`
- **我的印象**：刘老师的数值模拟工作和实验工作，是我复现的来源。
- 要点：有限偏移距垂直震电剖面（VSEP）配置下界面电磁波特征的理论建模与实验验证；理论公式来自 Schakel & Smeulders (2010)。

## 理论与复现关系

```text
Pride 1994 (PRB) ── Pride & Haartsen 1996 (JASA)        ← 理论基石
            │
            ▼
Schakel & Smeulders 2010 (JASA)                          ← 界面反射/透射公式（刘老师模拟的公式来源）
            │
            ├──► Schakel et al. 2011 (JAP)               ← 实验 + 模拟基石
            ▼
Liu et al. 2018 (JASA EL)                                ← 刘老师 VSEP 模拟 + 实验（复现来源）
```
