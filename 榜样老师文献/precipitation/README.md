# precipitation 文献（孔隙尺度混合诱导碳酸钙沉淀与溶解）

Werth（UIUC）、Valocchi 团队及其合作者（PNNL 的 Zhang 等，Sandia 的 Yoon 等）关于孔隙尺度混合诱导 CaCO3 沉淀/溶解的实验和模拟论文，按"论文名称 → 我的印象"整理。前两篇是一组：Zhang et al. (2010) 是微流控实验，Yoon et al. (2012) 是对标这组实验的孔隙尺度模拟。第三篇 Yoon et al. (2019) 是同一套微模型几何上的沉淀 + 溶解实验，引用了前两篇作对比。第四篇 Bate et al. (2026)（浙江大学团队）把同类横向混合沉淀的微流控实验与频谱激发极化（SIP）监测结合起来，引用了第 1、3 篇。第五篇 Peng et al. (2026)（瑞士 PSI 团队）不属于横向混合体系：硅胶毛细管反向扩散实验 + 三维 LBM 与神经网络形态计算，模拟 ACC 溶解与方解石/球霰石生长的耦合，引用了第 2、3 篇作为前人孔隙尺度模型和实验。第六篇 Rodriguez-Blanco et al. (2011)（利兹大学 Benning 团队）是均匀溶液中的批次结晶实验，不涉及孔隙介质：给出 ACC → 球霰石 → 方解石两阶段转化的动力学参数和机理，被第 5 篇引用，可作为本目录模拟工作的参数和机理来源。第七篇 Gebauer et al. (2008)（马普胶体与界面研究所 Cölfen 团队）也是均匀稀溶液中的实验，讲的是成核之前：碳酸钙在成核前就形成稳定团簇，团簇结合强度随 pH 变化，并与后续析出的 ACC 种类和最终晶型相对应；被第 5 篇引用，是非经典成核路线的源头文献。

## 一览

| 文件（论文名称） | 年份 / 期刊 | 我的印象 | PDF | SI |
|---|---|---|---|---|
| Pore-scale study of transverse mixing induced CaCO3 precipitation and permeability reduction in a model subsurface sedimentary system | 2010, ES&T | 微流控 CaCO3 沉淀实验的早期研究；有三维形貌表征方法（激光共聚焦）；可作为微流控实验来源的参考也是yoon2012实验来源 | [PDF](./Environmental%20Science%20and%20Technology%20-%202010%20-%20Zhang%20-%20Pore-scale%20study%20of%20transverse%20mixing%20induced%20CaCO3%20precipitation%20and%20permeability%20reduction.pdf) | [SI](./SI%20-%20Environmental%20Science%20and%20Technology%20-%202010%20-%20Zhang%20-%20Pore-scale%20study%20of%20transverse%20mixing%20induced%20CaCO3%20precipitation%20and%20permeability%20reduction.pdf) |
| Pore-scale simulation of mixing-induced calcium carbonate precipitation and dissolution in a microfluidic pore network | 2012, WRR | 结构严谨、论证详实的 CaCO3 沉淀模拟；写作引用、复现、学习写作三方面的强参考 | [PDF](./Water%20Resources%20Research%20-%202012%20-%20Yoon%20-%20Pore-scale%20simulation%20of%20mixing-induced%20calcium%20carbonate%20precipitation%20and.pdf) | 无 |
| Pore-scale analysis of calcium carbonate precipitation and dissolution kinetics in a microfluidic device | 2019, ES&T | 微流控 CaCO3 沉淀 + 溶解实验；模拟部分不完整，只是工作量补充；实验解释重点偏向反应表面积和反应速率 | [PDF](./Environmental%20Science%20and%20Technology%20-%202019%20-%20Yoon%20-%20Pore-scale%20analysis%20of%20calcium%20carbonate%20precipitation%20and%20dissolution%20kinetics%20in%20a%20microfluidic%20device.pdf) | [SI](./SI%20-%20Environmental%20Science%20and%20Technology%20-%202019%20-%20Yoon%20-%20Pore-scale%20analysis%20of%20calcium%20carbonate%20precipitation%20and%20dissolution%20kinetics%20in%20a%20microfluidic%20device.pdf) |
| Calcium carbonate precipitation visualization on a lab-on-a-chip model with spectral induced polarization monitoring | 2026, JGR Solid Earth | 微流控 CaCO3 沉淀实验 + SIP 监测；较好地解释了如何用 SIP 信号解读沉淀过程；与以往研究不同，除了熟化现象，还展示了后面的再沉淀堵塞过程 | [PDF](./JGR%20Solid%20Earth%20-%202026%20-%20Bate%20-%20Calcium%20Carbonate%20Precipitation%20Visualization%20on%20a%20Lab-on-a-Chip%20Model%20With%20Spectral.pdf) | 待补 |
| Bridging in-situ chemical imaging and pore-scale reactive transport modelling: mechanistic insight into CaCO3 polymorph dynamics | 2026, GCA | 研究碳酸钙熟化（ACC → 方解石/球霰石）的模拟；做了三维模拟；用 LBM + 神经网络求解地球化学 | [PDF](./Geochimica%20et%20Cosmochimica%20Acta%20-%202026%20-%20Peng%20-%20Bridging%20in-situ%20chemical%20imaging%20and%20pore-scale%20reactive%20transport%20modelling.pdf) | [SI](./SI%20-%20Geochimica%20et%20Cosmochimica%20Acta%20-%202026%20-%20Peng%20-%20Bridging%20in-situ%20chemical%20imaging%20and%20pore-scale%20reactive%20transport%20modelling.pdf) |
| The kinetics and mechanisms of amorphous calcium carbonate (ACC) crystallization to calcite, via vaterite | 2011, Nanoscale | 碳酸钙多晶型转变实验，实验数据详细、具体；有详细的动力学实验参数；提出了理论预测模型；可作为数值模拟的参数来源和机理解释来源 | [PDF](./Nanoscale%20-%202011%20-%20Rodriguez-Blanco%20-%20The%20kinetics%20and%20mechanisms%20of%20amorphous%20calcium%20carbonate%20(ACC)%20crystallization%20to%20calcite%2C%20via%20vaterite.pdf) | 无（原文无 ESI） |
| Stable Prenucleation Calcium Carbonate Clusters | 2008, Science | 非经典成核理论的奠基之作；做了非常基础的化学分析，讲清碳酸钙成核之前发生的故事；成核与 pH 紧密相关，不同 pH 对应最终产物的机制有待研究 | [PDF](./Science%20-%202008%20-%20Gebauer%20-%20Stable%20Prenucleation%20Calcium%20Carbonate%20Clusters.pdf) | [SI](./SI%20-%20Science%20-%202008%20-%20Gebauer%20-%20Stable%20Prenucleation%20Calcium%20Carbonate%20Clusters.pdf) |

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

### 3. Pore-scale analysis of calcium carbonate precipitation and dissolution kinetics in a microfluidic device

- 作者：Hongkyu Yoon, Kirsten N. Chojnicki, Mario J. Martinez（Sandia National Laboratories）
- 出处：Environmental Science & Technology 53(24), 14233–14242 (2019)，doi:10.1021/acs.est.9b01634
- 文件：`Environmental Science and Technology - 2019 - Yoon - Pore-scale analysis of calcium carbonate precipitation and dissolution kinetics in a microfluidic device.pdf`
- 支持材料（SI）：`SI - Environmental Science and Technology - 2019 - Yoon - ....pdf`，共 15 页：
  - Section S1：拉曼方法（Horiba LabRAM HR Evolution，532 nm，0–1200 cm⁻¹；方解石、文石、球霰石特征峰）；
  - Fig. S1–S12：微模型示意、全景图、三种共聚焦分辨率、分割流程、多孔/单孔高分辨率图、拉曼谱、2-D/3-D 对比、共聚焦切片；
  - Table S1：共聚焦成像参数（0.63/0.31/0.20 µm/pixel）；
  - Table S2：上、中、下游的 A2D 与 RSA 随时间变化（第二组列的表头印成了"Effective reaction rate"，从量级看应为 RSA，单位 µm²）；
  - 另有 Fig. S2、S5 高分辨率 pptx（未放入本目录）。
- 被引：Crossref 80 次（2026-11 查询）。
- **我的印象**：
  1. 做的是**微流控碳酸钙沉淀 + 溶解实验**；
  2. **模拟部分不完整，只是工作量的补充**：只在溶解 24 h 的固定几何上算一个快照（不更新矿物含量，原文 "without updating mineral contents"），用来定性解释溶解羽流，没有模拟溶解过程的时间演化，也没有和实测面积/速率做定量对比；
  3. 碳酸钙沉淀实验的**解释重点偏向反应表面积和反应速率**（几何 RSA vs 有效 RSA、有效速率 I_m 随时间的变化）。
- 要点：
  - 微模型：与 Zhang et al. (2010) 同一几何（2 cm × 1 cm，圆柱 300 µm，孔体 180 µm，孔喉 40 µm，孔隙度约 0.39），但深度 10 µm；Fig. S1 示意图标注 200 mm × 100 mm，应以正文 2 cm × 1 cm 为准。
  - 实验：CaCl2 与 Na2CO3 各 10 mM（pH 约 6 / 11），每个入口 50 µL/h（达西速度 1.67 cm/min）；出口另注 pH < 2 水防堵；沉淀阶段 75 h，然后两入口注 pH 4 水溶解约 150 h。
  - 成像：1 µm/pixel 光学拼图（多孔区域，插值到 0.2 µm 分析）；LSCM（Zeiss LSM510）单孔 3-D，竖向 1 µm 间隔，0.20 µm/pixel；拉曼鉴定 ACC、文石、方解石（本实验未见球霰石）。
  - 量化：总速率 = A2D × 10 µm / V_mol / dt（V_mol 按方解石 36.94 cm³/mol）；RSA = 周长 × 10 µm（只算竖向面）；有效速率 I_m = 总速率 / RSA 平均值。分割可重复性约 ±5%。
  - 结果：
    - 沉淀沿中线横向混合线生成，向下游展宽；上游孔隙堵塞后横向混合消失，中游混合线上移。
    - 分辨率：1 µm 图像明显低估 A2D 和 RSA，前人约 2–3 µm 的分析只能算定性。
    - 3-D：RSA3D/RSA2D 在位置 i 约 1.73、位置 v 约 1.06；体积 2-D 与 3-D 相近。
    - 速率：1.8 h 时 I_m = 1.4–3.0 × 10⁻⁵ mol/m²/s，与 k_r(1−SR) 量级一致，此时几何 RSA 可视为有效 RSA；3.1–75 h 间 RSA 变化在 ±24% 以内，下游 I_m 却降了约 2 个数量级，说明只有部分表面参与反应、反应受运移控制。
    - 溶解：上游 24 h 溶解速率 2.27 × 10⁻⁷ mol/m²/s，比文献方解石值高一个数量级，归因于不稳定晶型（文石、ACC）；上游溶解的离子在中下游再沉淀；溶解羽流出现在离沉淀物 2–3 个孔体处。
  - 模拟：沿用 Yoon et al. (2012) 的 LBM（Palabos）+ FVM 框架、Chou et al. (1989) 速率律；域 3.78 mm × 2.89 mm，1 µm 网格；三个情景：RSA × 2 + 方解石 K_sp、× 100 + 方解石、× 100 + 文石；只有第三个能复现沉淀线上方的溶解羽流。乘数 100 引自 Yoon et al. (2012)，本文没有独立标定，本质上是调参（注：本目录第 2 篇 README 记录的溶解因子是 d_f = 300，与这里说的 100 不同，引用时需核对）。
  - 作者承认的局限：洁净微模型早期生成 ACC，难以定量估算早期沉淀速率；建议改用方解石芯片（calcite chip）等表面矿物可控的装置。
- 作为参考的用法：
  - **写作引用**：几何反应表面积 ≠ 有效反应表面积、反应–水动力反馈、溶解羽流作为反应示踪剂、图像分辨率对孔隙尺度定量的影响。
  - **实验数据**：Table 1（总速率、有效速率）和 Table S2（A2D、RSA）给出了三个区域的时间序列，可直接用于模型对比。
  - **注意**：原文有几处不一致（Fig. 1c 写 130 h，Fig. S5 写 89 h；溶解速率正负号正文与 Table 1 相反；SI 中有"Figure SX"），引用数值时以表格为准。

### 4. Calcium carbonate precipitation visualization on a lab-on-a-chip model with spectral induced polarization monitoring

- 作者：Bate Bate, Lin-Han Wang, Yi-Xin Yang, Ke-Xin Chen, Long-Long Meng, Chi Zhang, Yun-Ming Chen, Sheng Zhou（浙江大学超重力研究中心、岩土工程研究所；维也纳大学）
- 出处：Journal of Geophysical Research: Solid Earth 131, e2026JB034544 (2026)，doi:10.1029/2026JB034544（2026-04 收稿，2026-09 接收）
- 文件：`JGR Solid Earth - 2026 - Bate - Calcium Carbonate Precipitation Visualization on a Lab-on-a-Chip Model With Spectral.pdf`
- 支持材料（SI）：Supporting Information S1，**尚未放入本目录（待补）**。正文引用了 Fig. S1–S10（S5 未被引用）：
  - Fig. S1：芯片孔隙度约 45%；
  - Fig. S2、S3：图像分割去噪；
  - Fig. S4：COMSOL 计算的几何因子 K = 5,152 m⁻¹；
  - Fig. S6：控制实验，排除电极极化和寄生电容伪影；
  - Fig. S7：相位谱演化；
  - Fig. S8、S9：m_n2 的 bootstrap 不确定性及其在堵塞阶段上移；
  - Fig. S10：天然介质中充电率与比表面积 S_por 的关系。
- 被引：2026 年新发表，暂未统计。
- 数据公开情况：原始数据和 MATLAB 图像处理脚本已公开在 Zenodo（doi:10.5281/zenodo.19520305）。
- **我的印象**：
  1. 做了**微流控碳酸钙沉淀实验，与 SIP 监测**同步进行；
  2. 论文**较好地解释了如何用 SIP 的信号去解读沉淀过程**（σ₀ 看导电通道是否被堵，m_n 看可接触的矿物–流体界面多少，τ 看极化单元尺度）；
  3. 与以往研究不同的点：**除了展示熟化现象，还展示了后面的再沉淀堵塞过程**，并把两个阶段分别对应到 SIP 参数的变化上。
- 要点：
  - 芯片：PDMS 软光刻，外形 60 × 25 × 2 mm，观察通道 35 × 10 × 0.2 mm；圆柱直径 600 µm，柱心距 800 µm，孔隙度约 45%；孔体积 31.5 µL。
  - 电极：芯片底部 4 块 150 nm 厚 Au 膜，ABMN 四电极，圆盘形接触；SIP 仪器 Ontash & Ermac；频率名义 0.1–10,000 Hz，1 Hz 以下数据因孔隙液化学非稳态而剔除。
  - 实验：先饱和 50 mM CaCl2，再从两个入口分别注入 50 mM CaCl2 与 50 mM Na2CO3，各 0.05 µL/min；1 PV = 315 min，共约 6 PV（约 31.5 h）；倒置显微镜 Nikon Eclipse Ti2，20× 物镜，延时拍摄后拼图。
  - 图像处理：MATLAB，0.6 µm/pixel；灰度化 → 增强去噪 → 反相 → 对比度拉伸 → 自适应阈值 → 形态学滤波与孔洞填充，去掉小于 2 像素的目标。
  - SIP 解释：双 Cole-Cole 模型（高频分量 1、低频分量 2），pyGIMLi 拟合，残差 bootstrap 评估不确定性；归一化充电率 m_n = σ₀·m/(1 − m)；Schwartz 关系 τ = d²/(8D) = 1/(2πf)。
  - 结果：
    - 熟化阶段（0–2 PV）：细小圆颗粒（类球霰石）与菱面体（类方解石）共存，细颗粒逐渐消失，菱面体长大（最大粒径约 10 → 30 µm），周围出现环状无沉淀带；m_n1 升高、τ₁ 增大、σ₀ 缓慢下降。
    - 堵塞阶段（2–6 PV）：流动和反应物输运重新分配，细颗粒二次成核、聚集，形成致密沉淀带（面积占比 2.8 PV 约 32% → 6.0 PV 约 54%）；σ₀ 骤降后稳定在约 2,000 µS/cm，m_n1 与 CaCO3 含量解耦而下降，m_n2 升高。
    - σ′₁Hz 分四阶段：2,830 → 2,588（Stage I）→ 2,556（Stage II）→ 急降（Stage III）→ 约 2,000 µS/cm 平台（Stage IV）。
    - σ″ 弛豫峰在 300–600 Hz；σ″_peak 由 7.2 升到约 29.0 µS/cm，再降到 17.6 µS/cm；f_peak 由 562 降到 312 Hz。
    - 汇总文献数据：m_n = 16904φ（R² = 0.85）优于 m = 6.31φ（R² = 0.57），也优于基于 S_por 的关系（不同方法估算的比表面积不代表电学有效界面）。
    - Schwartz 关系 τ = r²/(4.20 × 10⁻⁹)（R² = 0.84）适用于分散晶体；聚集体、胶结板、沉淀壁和其他介质偏离预测带。
  - 作者承认的局限：
    - 晶型（类球霰石、类方解石）只按形态、饱和度和多晶型路径推断，没有 XRD、FTIR 或 Raman 鉴定；
    - 残余电极极化、杂散电容和仪器相位误差不能完全排除，尤其是低频和约 1 kHz 以上的 σ″；
    - m_n2 不确定性大，只能作唯象指标，不能定量表示特征长度；
    - 缺少 ACC、球霰石的 Stern 层电荷密度数据，各晶型的极化强度按相同处理。
- 作为参考的用法：
  - **实验来源**：微流控 + SIP 联测的芯片设计、电极布置、几何因子标定和低频数据取舍。
  - **SIP 解释**：双 Cole-Cole 参数的物理意义，哪些可以定量（分散阶段的 m_n1、τ₁）、哪些只能定性（m_n2）；堵塞阶段可能叠加膜极化和 Maxwell-Wagner 极化，Cole-Cole 能拟合但参数不能再按颗粒极化解读。
  - **数据对比**：Fig. 5 汇总了大量文献的 σ″_peak 时间曲线、m–φ、m–S_por 和 τ–r 数据。
  - **与本目录对照**：本文引用了第 1 篇 Zhang et al. (2010) 和第 3 篇 Yoon et al. (2019)（环状无沉淀带的解释）。混合线沉淀堵塞在 Zhang et al. (2010) 中已经观察到，本文的新意在于把熟化和再成核堵塞两个阶段对应到 SIP 信号上，并解释了 σ″ 先升后降的形态原因。

### 5. Bridging in-situ chemical imaging and pore-scale reactive transport modelling: mechanistic insight into CaCO3 polymorph dynamics

- 作者：Haonan Peng（彭浩楠，一作兼通讯）, Ashish Rajyaguru, Enzo Curti, Daniel Grolimund, Sergey V. Churakov, Nikolaos I. Prasianakis（瑞士 PSI 放射性废物管理实验室 LES、瑞士光源 SLS；伯尔尼大学地质科学研究所）
- 出处：Geochimica et Cosmochimica Acta 418, 35–49 (2026)，doi:10.1016/j.gca.2026.02.029（2025-07 收稿，2026-02 接收；CC BY 开放获取）
- 文件：`Geochimica et Cosmochimica Acta - 2026 - Peng - Bridging in-situ chemical imaging and pore-scale reactive transport modelling.pdf`
- 支持材料（SI）：`SI - Geochimica et Cosmochimica Acta - 2026 - Peng - ....pdf`，共 4 页（第 4 页空白）：
  - Text S1：引导平衡（guided-equilibrium）D3Q27 LBM 的演化方程（式 S1），反应源项按格子权重分配 R_i = ω_i·Q_j（式 S2），浓度取零阶矩（式 S3）；
  - Text S2 + Fig. S1：155、156、157 h 时粗网格全域模拟与细网格子域模拟的 CaCl2/Na2CO3 浓度剖面对比（纯扩散），用来证明从粗网格提取的时变边界条件可用。
- 被引：OpenAlex 3 次、Semantic Scholar 2 次（2026-11 查询）；相关的只有 InterPore Journal 2026 的评述《Crystal Growth in Porous Media》（doi:10.69631/9kd53x06）。
- 数据公开情况：数据在 Mendeley Data（doi:10.17632/cp9tbz7cnz.2）；LBM 代码是 PSI 自编的 CUDA/C++ + MPI 程序，未开源。
- **我的印象**：
  1. 研究**碳酸钙熟化**的模拟（ACC → 方解石/球霰石）；
  2. 做了**三维模拟**；
  3. 用的是 **LBM + 神经网络求解地球化学**的方法。
- 对印象的补充说明（核对原文后）：
  - "熟化"要按广义理解：文中模拟的是 157.4–162.4 h 这 5 h 内 **ACC 溶解 → 释放 Ca²⁺/CO₃²⁻ → 扩散到邻近方解石、球霰石表面并使其继续生长**，即溶解–再沉淀式的晶型转化；**不包含同一晶相内部大颗粒吞并小颗粒的 Ostwald 熟化**，也不包含成核（晶体位置和初始形状直接取自实验）。球霰石 → 方解石的转化在这个时间窗口内也没有发生。
  - "三维"指的是三维 LBM 计算域（细网格 1400 × 32 × 32，0.01 mm），而实验数据是二维 X 射线吸收投影（像素 15 µm）；模型与实验对比的是投影图像和晶体体积。
  - "神经网络求解地球化学"具体是：前馈神经网络（3 层 × 12 神经元）替代 GEMS 做形态计算，输入 Na2CO3、CaCl2 浓度，输出 pH、a(Ca²⁺)、a(CO₃²⁻)；动力学速率仍用经验速率律另算，神经网络只管平衡形态。
- 要点：
  - 实验：硅胶充填玻璃毛细管（长约 80 mm、直径约 300 µm），两端储液池分别为 0.3 M CaCl2 + 0.1 M NaCl 和 0.3 M Na2CO3 + 0.1 M NaCl，反向扩散；在 SLS 做一周共 28 次 X 射线吸收扫描（平均间隔约 1.7 h），吸收信号按 CaCO3 线衰减系数（μ = 1.977 × 10⁻³ µm⁻¹，18.2 keV）换算成晶体体积；μ-XRD 定晶型（#1–5 为球霰石，#6 为方解石），μ-XRF 测元素分布。
  - 研究窗口：T_exp = 157.4–162.4 h（记为 T_sim = 0–5 h），重点是 #5（球霰石）、#6（方解石）和周围的 ACC。
  - 输运：D3Q27 引导平衡 LBM，纯扩散（u = 0）；表观扩散系数 D_a = δεD_w / [τ²(ε + ρ_b K_d)]，ε = 0.5、δ = 1.0、τ = 1.5、ρ_b = 1.02 g/cm³；K_d 按 pH 分段（pH < 6 为 0，6–8 为 10^(pH−10.1) 或 10^(pH−11.4)，> 8 为平台值 0.002 / 0.00073），取自 Peng et al. (2025, WRR) 的标定。
  - 化学：FNN 替代 xGEMS；训练集 153,664 个平衡计算点（浓度 10⁻¹⁰–0.3 M 对数网格），训练/验证/测试 = 80/10/10，MSE = 7.7 × 10⁻⁷；体系 pH 约 9.7–11，假设 CO₃²⁻ 代表全部碳的输运。
  - 动力学：Arvidson & Morse (2013) 通式 r± = A_s·k±·[±(1 − Ω)]^n，三相分别反演（Table 1）：方解石 k = 2.725 × 10⁻⁷ mol/m²/s、n = 1.34；球霰石 k = 6.23 × 10⁻⁸、n = 0.93；ACC 溶解 k = −2.90 × 10⁻⁶、n = 2.00。方解石 k 比 Busenberg & Plummer (1987) 的 (0.5–3.0) × 10⁻⁶ 低约一个数量级，作者用本体系 pCO₂ 极低（约 10⁻³·⁴ bar）解释（Fig. 7）。
  - 固相处理：方解石和球霰石按体素体积分数 φ_s 更新、只在固液界面生长；ACC 作为"半透、不堵塞"的相与溶液共存于同一体素，只降低局部扩散系数，不计入 φ_s。
  - 两级网格：粗网格全毛细管 2100 × 62 × 62（0.05 mm，约 8 × 10⁶ 体素）只算纯扩散，给细网格子域（x = −14–0 mm，1400 × 32 × 32，0.01 mm）提供时变边界条件。
  - 初始化三步：纯扩散算到 155.8 h → 放入实验重建的 157.4 h 固相，固定几何预跑到 157.4 h → 开启全耦合。
  - 结果：
    - 方解石和球霰石的体积、生长速率与实验吻合很好；ACC 在后期溶解偏快（Fig. 10）。
    - 机理（Fig. 11–13）：晶体快速生长消耗离子，使局部对 ACC 不饱和（方解石附近 SI_ACC 约 −1.0 到 −0.5），ACC 溶解释放的离子又扩散回去维持晶体生长，形成反馈。
    - 方解石旁的 ACC 先耗尽：162.4 h 时方解石沉淀速率降到约 2.0–4.0 × 10⁻⁵ mol/L/s（比峰值约 4.5 × 10⁻⁴ 低十倍以上），周围 pH 从约 10.5 降到约 9.8；球霰石左侧的 ACC 持续溶解起缓冲作用（pH 约 10.5，SI_VAT 约 2.5–3.0），所以球霰石朝 ACC 方向持续定向生长。
  - 计算效率：每个时间步的形态计算从约 0.4 h（GEMS 单核，约 143 万网格点）降到不到 1 s，提速超过 1400 倍；5 h 实验窗口在 CSCS Alps 上用 5 块 GPU 不到 40 min 算完。
  - 作者承认的局限：
    - ACC 溶解借用晶体的速率形式反演，只能算硅胶限域条件下的表观参数，不能直接和其他数据集比；
    - 初始浓度场是近似的，没有计入此前沉淀造成的离子耗竭；
    - 不包含成核，只能从实验给出的晶体位置开始（随机成核见 Peng et al. 2025 WRR）；
    - 后期 ACC 耗尽速率偏快，可能和孔隙度、局部输运的简化以及理想化的动力学有关。
- 我读时的疑点：
  - 细网格边界来自无反应的粗网格，反应造成的离子耗竭不会反馈到边界上；
  - 只用了两颗晶体和一个 5 h 窗口，而动力学参数又是用同一套数据反演的，"吻合"更接近拟合效果，不是独立预测；
  - 方解石附近 pH 降到约 9.8 时，HCO₃⁻ 的比例不小（pKa₂ ≈ 10.3），只用 CO₃²⁻ 代表碳的输运值得推敲；
  - 三维晶体和 ACC 几何如何由二维投影重建，正文交代得比较简略。
- 作为参考的用法：
  - **写作引用**：限域多孔介质中 ACC 作为溶质库驱动晶体生长、晶型特异性动力学、机器学习替代地球化学求解器、"数字孪生"辅助实验。
  - **方法参考**：两级网格（粗网格给边界）、预模拟初始化、FNN 替代形态计算的训练设置、用原位成像的体积时间序列反演速率参数。
  - **与本目录对照**：本文把第 2 篇 Yoon et al. (2012) 和第 3 篇 Yoon et al. (2019) 当作"二维、单一晶相、空间平均速率"的前人模型来对比。前四篇都是对流主导的横向混合沉淀，本文是纯扩散的反向扩散体系，而且明确区分 ACC、球霰石、方解石三相。第 2 篇推测的"球霰石 → 方解石重结晶、Ostwald 熟化加速溶解"，本文也没有直接模拟。
  - **同一团队的系列**：Peng et al. (2025, J. Hydrol.) 做输运反演和数字孪生 → Peng et al. (2025, WRR) 做成核 → 本文做成核之后的溶解–生长耦合。

### 6. The kinetics and mechanisms of amorphous calcium carbonate (ACC) crystallization to calcite, via vaterite

- 作者：Juan Diego Rodriguez-Blanco（通讯）, Samuel Shaw, Liane G. Benning（英国利兹大学地球与环境学院）
- 出处：Nanoscale 3(1), 265–271 (2011)，doi:10.1039/c0nr00589d（2010-08 收稿，2010-10 接收）
- 文件：`Nanoscale - 2011 - Rodriguez-Blanco - The kinetics and mechanisms of amorphous calcium carbonate (ACC) crystallization to calcite, via vaterite.pdf`
- 支持材料（SI）：无。原文首页没有 ESI 脚注，全文 8 张图、1 张表都在正文里。
- 被引：Crossref 1107 次（2026-11 查询）。
- 数据公开情况：没有数据可用性声明；α–时间曲线需要从 Fig. 3、5、6、7 数字化，拟合参数直接用 Table 1。
- **我的印象**：
  1. **碳酸钙多晶型转变**（ACC → 球霰石 → 方解石）的实验，实验数据非常详细、具体；
  2. 有**详细的动力学实验参数**（各温度的诱导时间、速率常数、拟合系数、活化能）；
  3. 提出了**理论预测模型**（式 4，给定温度和转化程度算所需时间）；
  4. 可以作为我们**数值模拟的参数来源**和**机理解释的来源**。
- 要点：
  - 实验：1 M Na2CO3 与 1 M CaCl2 等摩尔混合，80 mL 恒温搅拌 Teflon 反应池，7.5、10、20、25 °C 四个温度；Daresbury SRS 16.4 线站原位 ED-XRD，每 15 s–1 min 一张谱，最长跟踪 20 h，XFIT 拟合峰面积并归一化为反应程度 α（0–1）。离线取样做 XRD（Bruker D8）、FTIR（ATR，650–4000 cm⁻¹）、FEG-SEM（LEO 1530，3 keV）；PHREEQC（wateq4f）算饱和指数。
  - 两阶段路径（Fig. 1、3）：阶段 1 为 ACC → 球霰石，快；阶段 2 为球霰石 → 方解石，约慢 10 倍。7.5 °C 时阶段 1 约 1 h，阶段 2 约 17 h；终产物只有方解石。
  - 阶段 1 机理（Fig. 2、4a–e、5）：
    - ACC 为小于 50 nm 的近球形颗粒，含结构水（FTIR 的 O–H 带，含水量可达约 18 wt%）。
    - ED-XRD 背景强度（代表 ACC）下降与球霰石 (101) 峰生长耦合；背景下降比球霰石峰早约 14 min（7.5 °C）。ACC 分解完毕：7.5 °C 约 45 min，25 °C 约 12 min。
    - 球霰石由与 ACC 尺寸相近、无晶面的纳米亚单元聚集而成。作者推断为"ACC 快速脱水 → 颗粒内部结构重组 → 聚集"，不是溶解后从溶液析出（推断，有 Goodwin et al. 2010 的结构旁证）。
  - 阶段 2 机理（Fig. 4f–i、6、7）：
    - 驱动力：球霰石 Ksp = 10⁻⁷·⁹¹³ > 方解石 Ksp = 10⁻⁸·⁴⁸⁰，只要球霰石在，溶液就对方解石过饱和。
    - 球霰石消失和方解石生长都自加速；方解石长在球霰石团聚体表面，终产物留下球形"铸模"。作者据此认为是溶解–再沉淀、受方解石表面积控制的过程（原文称为 hypothesis）。
  - 动力学模型：用 Ogino et al. (1990) 模型拟合方解石生长：
    - 式 (1)：α = (b(t − t₀) + c)³；式 (2)：b = k·fₓ·A₀^(−2/3)·s₀/3；式 (3)：fₓ = (IAP)^½ − (Ksp)^½，IAP 取球霰石 Ksp（假设溶液对球霰石饱和）。
    - 25 °C 的 k 固定为 Ogino 值 2.67 × 10² s⁻¹，反推 s₀ = 0.188 m²；按菱面体、密度 2.71 g/cm³ 算出 t₀ 时方解石粒径 0.63 µm（SEM 为 0.5–1 µm），再假设各温度初始粒径相同，求出各温度的 k。
  - Table 1 参数（方解石）：

    | T / °C | t₀ / s | k (×10² s⁻¹) | b (×10⁻⁶) | c |
    |---|---|---|---|---|
    | 7.5 | 5100 | 0.71 | 2.10 | 0.0805 |
    | 10 | 2880 | 0.86 | 3.52 | 0.1013 |
    | 20 | 936 | 2.19 | 7.18 | 0.0719 |
    | 25 | 792 | 2.67（固定为 Ogino 值） | 7.66 | 0.0724 |

    另有 Ogino (1990) 的 k：30 °C 4.67、40 °C 11.0、50 °C 28.3、60 °C 58.3（×10² s⁻¹）。
  - 活化能（Fig. 8，Arrhenius）：成核 Ea = 73 ± 10 kJ/mol（lnA = 23 ± 4，由 t₀ 求）；生长 Ea = 66 ± 2 kJ/mol（lnA = 32 ± 1，本文与 Ogino 数据合并，R² > 0.99）。
  - 预测模型式 (4)：t = exp(−23.2 + 8862/T) + ∛(α − c)/b（t 单位 s，T 单位 K，b、c 取 Table 1）。适用于纯 ACC、低于 30 °C；约 40 °C 以上生成文石。预测环境温度下纯 ACC 完全转化为方解石需约 4–16 h。
  - 作者承认的局限：海胆骨针中的转化要数天且无球霰石（Beniash et al. 1997），作者推测是 Mg（约 5%）或有机质的影响，所以模型只适用于纯体系。
- 我读时的疑点：
  - 阶段 1 正文说球霰石亚单元"小于"ACC 颗粒，但给的数值是 30–70 nm 对 20–45 nm，数值和说法相反；
  - 写 66 kJ/mol"落在表面控制反应的范围（< 34 kJ/mol）内"，字面自相矛盾，可能是笔误；
  - 式 (4) 的 ∛(α − c) 与式 (1) 反解得到的 α^(1/3) − c 不一致，用式 (4) 前要先按式 (1) 自己推一遍；
  - 模型适用温度上限：摘要写 7.5–40 °C，正文写低于 30 °C；
  - 各温度的 k 依赖"25 °C 的 k 取文献值"和"初始粒径都是 0.63 µm"两个假设，不是独立测得的；
  - 阶段 1 只给了时间尺度，没有给速率常数或活化能。
- 作为参考的用法：
  - **模拟参数**：方解石生长速率常数 k(T)、诱导时间 t₀(T)、活化能（成核 73、生长 66 kJ/mol）、球霰石与方解石的 Ksp；α–时间曲线可数字化后用来标定或验证模型。
  - **机理解释**：ACC 脱水原位转化为球霰石、球霰石溶解–再沉淀为方解石、生长速率受方解石表面积控制，可用来解释模拟中的多晶型演化和速率自加速。
  - **与本目录对照**：第 5 篇 Peng et al. (2026) 引用了本文，并在模拟中区分 ACC、球霰石、方解石三相；第 1 篇 Zhang et al. (2010) 观察到以球霰石为主、伴有方解石；第 2 篇 Yoon et al. (2012) 推测的"球霰石 → 方解石重结晶"可以用本文的溶解–再沉淀机理和时间尺度来对照。需要注意，本文是 1 M 高浓度、搅拌、均匀溶液的批次实验，用到孔隙尺度、低浓度、输运控制的体系时要考虑条件差异。

### 7. Stable Prenucleation Calcium Carbonate Clusters

- 作者：Denis Gebauer（一作）, Antje Völkel, Helmut Cölfen（通讯，coelfen@mpikg.mpg.de）（德国马普胶体与界面研究所，Potsdam-Golm）
- 出处：Science 322(5909), 1819–1822 (2008)，doi:10.1126/science.1164271（2008-08 收稿，2008-11 接收）
- 文件：`Science - 2008 - Gebauer - Stable Prenucleation Calcium Carbonate Clusters.pdf`
  - 注意：这是从 science.org 下载的期刊版面，共 5 页：第 1 页上半部分是前一篇论文的参考文献，第 4 页下半部分是下一篇论文（Knudson et al., Shock-Wave Exploration of the High-Pressure Phases of Carbon）的开头，第 5 页是下载封面。本文正文在第 1–4 页。
- 支持材料（SI）：`SI - Science - 2008 - Gebauer - Stable Prenucleation Calcium Carbonate Clusters.pdf`，共 34 页：
  - Section 1：材料与方法（Metrohm Titrando 809 / 800 Dosino 恒 pH 滴定系统，钙离子选择电极 6.0508.110，电极校准，实验条件）；
  - Section 2.1：由恒 pH 滴定的 NaOH 用量换算结合碳酸根（式 [1]–[10]）；
  - Section 2.2：结合钙与结合碳酸根对比（团簇平均 1:1、电中性）；
  - Section 2.3：分析超速离心（AUC）检测团簇；
  - Section 2.4：多重结合模型（式 [13]–[19]，参数 x、K、K′）；
  - Section 2.5–2.7：离子积、计入团簇后的过饱和比、草酸钙与磷酸钙的对照实验；
  - Fig. S1–S15 和 Table S1（AUC 中三种团簇的 s、D 和粒径）。
- 被引：OpenAlex 1830 次（2026-11 查询）。
- 数据公开情况：没有数据可用性声明，曲线需要从图中数字化；结合参数（x、K）、溶度积和 AUC 结果在 SI 正文和 Table S1 中直接给出。
- **我的印象**：
  1. **非经典成核理论的奠基之作**；
  2. 做了**非常基础的化学分析**（钙离子选择电极 + 恒 pH 滴定 + 质量守恒），讲清了**碳酸钙在成核之前发生的故事**；
  3. 碳酸钙的**成核与 pH 紧密相关**，其中**不同 pH 对应最终产物（的机制）有待研究**。
- 对印象的补充说明（核对原文后）：
  - "不同 pH 对应什么产物"本文其实已经给出了观测：pH 9.00–9.50（团簇内结合强）析出 ACC I，最终以方解石为主；pH 9.75–10.0（结合弱）析出 ACC II，最终以球霰石为主；没有检出文石（Fig. 3、Fig. S11、S13）。**有待研究的是机理**：团簇结构如何决定 ACC 种类、ACC 与晶型的选择受热力学还是动力学控制，原文明确说"仍然未知"。
  - "非经典成核"的图景在本文之后一直有争论（团簇是否真为稳定物种、能否用液–液分相或经典理论解释），引用时宜写作"提出了成核前稳定团簇的观点"，不要写成定论。
- 要点：
  - 实验：25 mL、10 mM 碳酸盐缓冲液（pH 9.00、9.25、9.50、9.75、10.0），(24 ± 1) °C，以 10 µL/min 滴入 10 mM CaCl2（即 0.1 µmol/min）；10 mM NaOH 恒 pH 滴定；钙电极测游离 Ca²⁺；每个 pH 三次重复（Fig. S1、S2）。
  - 结合钙 = 加入量 − 游离量。成核前（包括欠饱和阶段）就有钙被结合：pH 9.00 约 35%（缓冲液中 CO₃²⁻ 约 4%），pH 10.0 约 75%（CO₃²⁻ 约 25%）（Fig. 1）。
  - 成核前游离钙随时间线性上升，成核后停在溶解度水平；作者据此认为团簇是溶质（活度不为 1），按平衡热力学形成，是热力学稳定的，而不是经典理论中的亚稳团簇（Fig. 2 为示意，能量低谷深度和成核势垒高度未知）。
  - 结合碳酸根与结合钙在实验精度内相等，团簇平均为中性的 1:1（Fig. S4、S5；碳酸根曲线做了偏移和斜率校正）。
  - AUC（pH 9.00）：过饱和和接近成核时检出 cluster I（约 2 nm，约 70 个离子），统计显著性较低的 cluster II（约 4 nm），成核后早期有 cluster III（约 5–6 nm）。作者推测成核是团簇聚集（Fig. S6、Table S1）。
  - 多重结合模型（Fig. S7、S8、S10）：x 为一个碳酸根平均结合的钙数，K 为单个结合的平衡常数；pH 9.00：x = 1.05，K = 1350 M⁻¹；pH 10.0：x = 1.47，K = 713 M⁻¹。宏观结合常数 K′ = x·K，Δ_RG° = −RT ln K′，约 −17 到 −18.5 kJ/mol（Fig. S11）。
  - 两种 ACC：溶度积约 3.1 × 10⁻⁸ M²（ACC I）和约 3.8 × 10⁻⁸ M²（ACC II），分界在 pH 9.50 与 9.75 之间（Fig. 3）；偏光显微镜确认最先析出的是无定形相（Fig. S12）；WAXS 确认最终晶型（Fig. S13）。
  - 忽略团簇时，过饱和比被高估约 40%（pH 9.00）到约 75%（pH 10.0）（Fig. S14）。
  - 在 pH 8.0 的磷酸钙、草酸钙体系中定性看到同样的成核前钙结合（Fig. S15）。
- 作者承认的局限：
  - 团簇的尺寸分布、结构、能量低谷深度和成核势垒高度都未知；
  - 成核是团簇聚集还是单离子附着生长，未定（作者倾向于聚集）；
  - K′ 不描述整个团簇 z·Ca²⁺ + z·CO₃²⁻ ⇌ {CaCO₃}_z 的平衡，团簇浓度和 z 无法得到；
  - 多重结合模型假设所有结合位点等同且独立，只适用于成核前；
  - AUC 在欠饱和阶段测不到团簇，成核后小团簇测不到也可能只是浓度太低；
  - 熵驱动的溶剂（水合）效应只是推测（原文用 "speculatively"）。
- 我读时的疑点：
  - pH 9.50 与 9.75 按拟合点算出的 K′ 几乎相同（约 1112 与 1121 M⁻¹），却分属 ACC I 和 ACC II，分组更多依赖插值曲线；
  - 碳酸根曲线的斜率校正是按成核后 1:1 定的，所以成核后的 1:1 是前提而不是结果；
  - SOM 2.4 末段写"示于 Figure S10"，按内容应为 Fig. S11。
- 作为参考的用法：
  - **写作引用**：成核前稳定团簇、非经典成核路径、ACC 作为前驱相、pH 对多晶型选择的影响；计入团簇后成核驱动力（过饱和度）被高估的问题。
  - **机理解释**：模拟或实验中出现 ACC、球霰石、方解石共存或随 pH 变化时，可用本文的"团簇结合强度 → ACC I/II → 方解石/球霰石"对应关系作背景。
  - **与本目录对照**：第 5 篇 Peng et al. (2026) 引用了本文，并在其前篇（Peng et al. 2025 WRR）中考虑了非经典成核；第 6 篇 Rodriguez-Blanco et al. (2011) 讲的是本文之后的阶段（ACC → 球霰石 → 方解石的转化动力学）。本文是 10 mM 稀溶液、pH 9–10、缓慢加钙的均匀体系，用到孔隙尺度混合沉淀（第 1–4 篇为 6.5–50 mM 的 CaCl2 与 Na2CO3 两股溶液直接混合）时要注意条件差异。

## 相关文献（未放 PDF）

| 论文 | 出处 | 说明 |
|---|---|---|
| Yoon, Kang & Valocchi, Lattice Boltzmann-based approaches for pore-scale reactive transport | Rev. Mineral. Geochem. 80, 393–431 (2015) | 同一团队的 LBM 反应输运综述，重写代码时可参考 |
| Peng et al., Machine learning-enhanced modeling of calcium carbonate nucleation in porous media under counter-diffusion conditions | Water Resour. Res. 61(11), e2025WR040484 (2025)，doi:10.1029/2025WR040484 | 第 5 篇的前篇，同一套反向扩散实验的成核阶段（经典 + 非经典成核、随机诱导期） |
| Peng et al., Towards digital twin of an in-situ experiment: a physics-enhanced machine-learning framework for inverse modelling of mass transport processes | J. Hydrol. 664, 134437 (2026)，doi:10.1016/j.jhydrol.2025.134437 | 第 5 篇的输运反演和数字孪生框架 |
| Prasianakis et al., Neural network based process coupling and parameter upscaling in reactive transport simulations | Geochim. Cosmochim. Acta 291 (2020)，doi:10.1016/j.gca.2020.07.019 | 第 5 篇神经网络替代形态计算的来源 |
| Bots et al., Mechanistic insights into the crystallization of amorphous calcium carbonate (ACC) | Cryst. Growth Des. 12(7) (2012)，doi:10.1021/cg300676b | 原位 SAXS/WAXS；ACC → 球霰石三阶段，第三阶段为球霰石 Ostwald 熟化（第 5 篇引用） |
| Shen et al., Properties of amorphous calcium carbonate and the template action of vaterite spheres | J. Phys. Chem. B 110(7) (2006)，doi:10.1021/jp055063o | CaCl2 + Na2CO3 快速混合生成 ACC，再转化为球霰石/方解石（第 5 篇引用） |
