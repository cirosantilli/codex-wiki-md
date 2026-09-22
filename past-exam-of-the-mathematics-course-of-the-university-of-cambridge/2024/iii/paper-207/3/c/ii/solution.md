<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For component $m$, stack its $N_m$ assigned observations as $y_1^{(m)},\ldots,y_{N_m}^{(m)}\in\mathbb R^n$. The prior is $f_m\sim N_n(0,K)$ and each assigned vector is conditionally $N_n(f_m,\sigma^2I_n)$. [Normal-normal conjugacy](../../../../../../../normal-normal-conjugacy-with-known-observation-variance.md) gives

$$
f_m\mid y,c,\pi\sim N_n(\mu_m,V_m),
$$

where

$$
V_m=\left(K^{-1}+\frac{N_m}{\sigma^2}I_n\right)^{-1},
\qquad
\mu_m=V_m\frac1{\sigma^2}\sum_{r=1}^{N_m}y_r^{(m)}.
$$

If $N_m=0$, this reduces to the prior $N_n(0,K)$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
