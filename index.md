<script type="text/javascript" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"> </script>

# 2024-Fall-Numerical-solution-for-Partial-Differential-Equations

- 课堂教学、随堂练习
- 作业：书面作业（每周交一次，周一交）；程序作业（布置作业后隔一周交，周四交）
- 总成绩 = 期末考试成绩 + 随堂练习 + 作业 （无期中考试）

#### 引言
- 四大科学方法：理论推导、物理实验、科学计算、机器学习
  - 用“理论推导”求解实际问题
$$
\text{实际问题} \xrightarrow{\text{简化}} \text{物理模型} \xrightarrow{} \text{数学模型} \xrightarrow{\text{理论推导}} \text{精确解} \xrightarrow{} \text{解的有效分析}
$$
  - 用“物理实验”求解实际问题
$$
\text{实际问题} \xrightarrow{\text{可在实验室执行的}} \text{物理模型} \xrightarrow{} \text{实验结果} \xrightarrow{} \text{近似解} \xrightarrow{} \text{解的有效分析}
$$
  - 用“机器学习”求解实际问题（数据无限好+算力无限大=理论上可以解决所有问题）
$$
\text{实际问题} \xrightarrow{} \text{数据} \xrightarrow{} \text{机器学习} \xrightarrow{} \text{近似解} \xrightarrow{} \text{解的有效分析}
$$
  - 用“科学计算”求解实际问题
$$
\text{实际问题} \xrightarrow{\text{简化}} \text{物理模型} \xrightarrow{} \text{数学模型} \xrightarrow{\text{数值近似}} \text{近似解} \xrightarrow{} \text{解的有效分析}
$$
- 部分数学模型：控制方程（组）（如：偏微分方程）+ 定解条件
- 如何确认解的有效性：将方法用到简化模型或有准确解的模型上，或与物理实验结果比较
- 适定问题：如果定解问题的解存在唯一，且关于定解条件是稳定的，则称该问题是适定的
- 求解步骤：时间区域剖分 → 偏微分方程（组）离散 → 定解条件（初边值）离散 → 求解离散方程组（数值代数）→ 结果分析, 讨论 → 有效可靠的数值解
- 常用的偏微分方程数值方法：有限差分法、有限元方法、谱方法
