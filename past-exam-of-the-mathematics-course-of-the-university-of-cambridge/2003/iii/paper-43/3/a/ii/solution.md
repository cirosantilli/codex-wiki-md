<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Hold all parameters except $\mu_i$ fixed and propose $\mu_i'=\mu_i+\eta$ with $\eta\sim N(0,s_{\mu i}^2)$. This [Random-walk Metropolis algorithm](../../../../../../../random-walk-metropolis-algorithm.md) has a symmetric [proposal distribution](../../../../../../../proposal-distribution.md). Define

$$
D_j'=D_j+\omega_i\{\varphi(x_j;\mu_i',v_i)-\varphi(x_j;\mu_i,v_i)\}.
$$

Cancellation of unchanged likelihood and prior factors gives the [Metropolis–Hastings acceptance probability](../../../../../../../metropolis-hastings-acceptance-probability.md)

$$
\boxed{a_i=\min\left\{1,\ \prod_{j=1}^n\frac{D_j'}{D_j}\exp\left[-\frac{(\mu_i')^2-\mu_i^2}{2\tau^2}\right]\right\}.}
$$

Draw an independent uniform and accept if it is at most $a_i$; otherwise retain the old value. Update each component in turn, recomputing the needed mixture contributions. On a logarithmic scale, compare $\log U$ with $\min(0,\sum_j\log(D_j'/D_j)-[(\mu_i')^2-\mu_i^2]/(2\tau^2))$ to avoid numerical underflow.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
