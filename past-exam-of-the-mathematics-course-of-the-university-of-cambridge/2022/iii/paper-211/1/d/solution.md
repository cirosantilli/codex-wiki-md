<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let

$$
D_t=\sum_{s=1}^t\frac{\delta_s}{N_s},
\qquad D_0=0,
$$

where the sum is componentwise, and set

$$
K_t=H_t+\eta_t(H_t\cdot D_{t-1}).
$$

Then

$$
X_t^{x,K}
=H_t\cdot(\delta_t+P_t)+N_tH_t\cdot D_{t-1}
=H_t\cdot\widetilde P_t
=\widetilde X_t^{x,H}.
$$

Also $K_{t+1}\cdot P_t=H_{t+1}\cdot\widetilde P_t$, so subtracting the new holdings value gives $C_t^{x,K}=\widetilde C_t^{x,H}$.

## ↑ Ancestors (11)

1. [D](../d.md)
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
