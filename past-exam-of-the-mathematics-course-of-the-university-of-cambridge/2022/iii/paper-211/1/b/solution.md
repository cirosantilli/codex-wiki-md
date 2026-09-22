<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $V_t=X_t^{x,H}-C_t^{x,H}=H_{t+1}\cdot P_t>0$. Set $a_0=1$ and recursively

$$
a_t=a_{t-1}\frac{X_t^{x,H}}{V_t},
\qquad
\eta_{t+1}=a_tH_{t+1}.
$$

The factors are positive and adapted, so $\eta$ is previsible. For $t\geq1$,

$$
X_t^{\nu,\eta}=a_{t-1}X_t^{x,H}
=a_tV_t=\eta_{t+1}\cdot P_t,
$$

while the same identity at $t=0$ defines $\nu=\eta_1\cdot P_0$. Thus consumption is zero and wealth is strictly positive, so $\eta$ is a [numéraire portfolio](../../../../../../numeraire-portfolio.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
