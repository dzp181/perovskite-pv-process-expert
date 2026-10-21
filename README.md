# 钙钛矿光伏工艺专家（Perovskite PV Process Expert）

<p align="left"><img src="avatars/expert.png" width="140" alt="Perovskite PV Process Expert"></p>

钙钛矿电池与组件全流程工艺专家：前驱体配方与狭缝涂布、结晶退火控制、P1-P4 激光划刻与死区优化、传输层与电极沉积、封装阻隔与湿热可靠性、叠层集成与产线良率排障。

WorkBuddy 专家包（Agent 型），标识 `perovskite-pv-process-expert`，行业分类 `02-Engineering`。

## 快速安装

下载 [`perovskite-pv-process-expert.zip`](./perovskite-pv-process-expert.zip)（或 Releases 中的附件）解压到专家目录：

```bash
unzip perovskite-pv-process-expert.zip -d ~/.workbuddy/plugins/marketplaces/my-experts/plugins/
```

重启 / 刷新 WorkBuddy，在【专家中心 - 我的专家】即可看到「钙钛矿光伏工艺专家」。

## 类型

Agent 型（单个 AI 专家）

## 功能

- **前驱体配方与溶剂体系**：PbI₂/FAI/MAI/CsI 化学计量与相稳定（黑相/黄相）、DMF-DMSO-NMP 配比、1.3–1.6 M 浓度窗口、添加剂与过饱和度—晶粒—缺陷的定量关系、前驱体老化与过滤。
- **成膜与大面积均匀性**：刮涂/狭缝涂布/喷涂/双源蒸镀工艺窗口、干燥速率与残余应力、Marangoni 对流花纹（"香蕉纹"）、膜厚均匀性验收、旋涂到狭缝的工艺迁移难点。
- **结晶与退火动力学**：反溶剂诱导结晶、气淬、蒸气退气、热板退火曲线、成核—生长竞争、迁移能垒与晶界加速效应（FAPbI₃ 黑相稳定化、划刻沟槽内结晶调控、激光退火快速结晶）。
- **传输层与电极工艺**：SnO₂/TiO₂/PTAA/2PACz+Al₂O₃/C₆₀/PCBM 成膜与能级对齐、Spiro-OMeTAD 掺杂与氧化、Au/Ag/Cu 电极蒸镀、AgI 生成导致的串联电阻上升。
- **激光划刻与死区控制**：P1–P4 目标层与波长选择（1064 nm 对 TCO、532/355 nm 冷消融）、能量密度与脉冲重叠率窗口、死区与 GFF 的定量关系、划刻套准精度、P1 沟槽积液与边缘 PbI₂ 富集。
- **封装与铅风险管理**：POE/EVA + 丁基胶边缘密封方案、WVTR/OTR 指标、ALD 无机阻挡层、边缘发白与分层排障、铅螯合与离子交换树脂固定、IEC 63163 铅释放要求。
- **可靠性与失效分析**：IEC 61215/61730/61701/63163、湿热 85/85 1000–3000 h、热循环、光浸泡 MPP 追踪、T80 衰减外推；EL/PL mapping、ToF-SIMS 离子分布、XRD 相分析、截面 SEM 等表征手段选型。
- **叠层集成**：宽带隙顶电池设计（Eg 1.68–1.78 eV）、绒面 TOPCon/HJT 上的钙钛矿沉积、TCO 透明复合电极、电流匹配、叠层效率纪录跟踪。
- **产线爬坡与成本建模**：GW 产线设备选型与国产化率、节拍与 OEE、良率损失树与 SPC 管控、BOM 拆解（电极 37% / 玻璃封装 32% / 前驱体 5%）、单瓦成本测算与降本排序。

## 使用示例

- 我有一条 2.78m² 的钙钛矿叠层组件产线，大面积涂布后效率只有 22% 不到，帮我按前驱体、涂布、划刻、封装逐环节定位问题。
- 我们的钙钛矿组件过了 IEC 61215，但户外 6 个月还是出现边缘发白和分层，水到底是从哪里进去的？
- 帮我设计一个钙钛矿/晶硅叠层的顶电池：带隙怎么定、传输层选什么、当前的效率与稳定性基准是多少？

## 头像

头像已自动生成在 `avatars/expert.png`（512×512，PNG）。如需替换为自定义头像，要求：
- 格式：PNG（推荐）或 JPG
- 尺寸：512×512 px
- 大小：单张不超过 500KB

## 安装

将专家包目录放到专家目录下：

```
/Users/dzp/.workbuddy/plugins/marketplaces/my-experts/plugins/perovskite-pv-process-expert/
```

然后运行注册命令使其可见：

```bash
python3 scripts/register_expert.py <expert-dir>
```

## 打包分享

```bash
python3 scripts/package_expert.py <expert-dir>
```

## 免责声明

本专家包中的效率纪录、成本区间与工艺参数基于截至 2026 年 10 月的公开资料整理，用于工程量级判断与检索方向指引；实际取值须以具体设备、具体材料规格书与现行有效标准为准，不构成认证、合规或投资结论。
