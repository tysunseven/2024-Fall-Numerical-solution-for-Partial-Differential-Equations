<script type="text/javascript" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"> </script>
# 2024-Fall-Numerical-solution-for-Partial-Differential-Equations

- 课堂教学、随堂练习
- 作业：书面作业（每周交一次，周一交）；程序作业（布置作业后隔一周交，周四交）
- 总成绩 = 期末考试成绩 + 随堂练习 + 作业 （无期中考试）
- 本课程研究的问题
- 三（四？）大科学方法：理论推导、物理实验、（大）科学计算、机器学习（？）
  - 用“理论推导”求解实际问题
\[
\text{实际问题} \xrightarrow{\text{简化}} \text{物理模型} \xrightarrow{} \text{数学模型} \xrightarrow{\text{理论推导}} \text{精确解} \xrightarrow{} \text{解的有效分析}
\]
  - 用“物理实验”求解实际问题
\[
\text{实际问题} \xrightarrow{\text{可在实验室执行的}} \text{物理模型} \xrightarrow{} \text{实验结果} \xrightarrow{} \text{近似解} \xrightarrow{} \text{解的有效分析}
\]
  - 用“机器学习”求解实际问题（数据无限好+算力无限大=理论上可以解决所有问题）
\[
\text{实际问题} \xrightarrow{} \text{数据} \xrightarrow{} \text{机器学习} \xrightarrow{} \text{近似解} \xrightarrow{} \text{解的有效分析}
\]
  - 用“科学计算”求解实际问题
\[
\text{实际问题} \xrightarrow{\text{简化}} \text{物理模型} \xrightarrow{} \text{数学模型} \xrightarrow{\text{数值近似}} \text{近似解} \xrightarrow{} \text{解的有效分析}
\]
- 部分数学模型：控制方程（组）（如：偏微分方程）+ 定解条件
- 如何确认解的有效性：将方法用到简化模型或有准确解的模型上，或与物理实验结果比较
- 偏微分方程（组）分类（按线性、非线性分类）
  - 线性PDE：对未知函数及其在方程（组）中出现的所有偏导数都是线性的，如：\\(u_t+a(x,t)u_x=(c(x,t)u_x)_x\\)
  - 非线性PDE：除线性PDE以外的PDE；如： \\(u_t+uu_x=(uu_x)_x\\)
  - 拟线性PDE：对未知函数在方程（组）中出现的最高阶偏导数是线性的，如：\\(u_t+uu_x=(c(x,t)u_x)_x\\)
- 常见的模型方程
  1.  对流方程（双曲型方程）
$$u_t+a(x,t)u_x=0,\quad u_t+uu_x=0$$

  2.  热传导方程（抛物型方程、扩散方程）

$$ u_t=c(x,t)u_{xx} $$

  1.  对流扩散方程
$$ u_t+a(x,t)u_x=c(x,t)u_{xx} $$
  1.  波动方程（双曲型方程）
$$ u_{tt}=c^2u_{xx} $$
  1.  Poisson方程
$$ u_{xx}+u_{yy}=f(x,y) $$
  1.  KdV方程
$$ u_x+uu_x+\delta u_{xxx}=c(x,t) $$
  1.  Euler方程