<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a time-homogeneous [continuous-time multi-state model](../../../../../../continuous-time-multi-state-model.md) with states $H$ (healthy), $I$ (ill), and $D$ (dead), where $D$ is absorbing. For risk-factor indicator $z\in\{0,1\}$, let the transition intensities be

$$
H\xrightarrow{\lambda_z}I,
\qquad
I\xrightarrow{\gamma}H,
\qquad
I\xrightarrow{\delta}D,
\qquad
\lambda_z=\lambda_0e^{\beta z}.
$$

Here $\lambda_0$ is the infection rate without the risk factor, $e^\beta$ is the infection [hazard ratio](../../../../../../hazard-ratio.md), $\gamma$ is the recovery rate, and $\delta$ is the disease-death rate. The assumption that the risk factor affects only acquisition makes $\gamma$ and $\delta$ common to both groups. The [infinitesimal generator](../../../../../../infinitesimal-generator-stochastic-processes.md) is

$$
Q_z=
\begin{pmatrix}
-\lambda_z&\lambda_z&0\\
\gamma&-(\gamma+\delta)&\delta\\
0&0&0
\end{pmatrix}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
