<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put

$$
A_t=\sum_{s=0}^t\frac{C_s^{x,H}}{N_s},
\qquad A_{-1}=0,
$$

and define

$$
K_t=H_t+A_{t-1}\eta_t
\quad(t\geq1).
$$

Because the numéraire strategy is self-financing,

$$
X_t^{x,K}=X_t^{x,H}+A_{t-1}N_t.
$$

Moreover,

$$
\begin{aligned}
C_t^{x,K}
&=X_t^{x,H}+A_{t-1}N_t
-H_{t+1}\cdot P_t-A_t\eta_{t+1}\cdot P_t\\
&=C_t^{x,H}+N_t(A_{t-1}-A_t)=0.
\end{aligned}
$$

This also proves the required wealth formula.

## ↑ Ancestors (11)

1. [C](../c.md)
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
