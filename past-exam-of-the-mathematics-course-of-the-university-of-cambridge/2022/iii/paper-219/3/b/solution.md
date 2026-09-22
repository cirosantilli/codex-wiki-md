<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $c_s=\widetilde c_s-E_s$ and $M_s=\widetilde M_s-RE_s$. With the stated [improper hyperpriors](../../../../../../improper-prior.md), the unnormalized [posterior density](../../../../../../posterior-density.md) is

$$
\begin{aligned}
&p(\{E_s\},M_0,c_0,\beta,\sigma_M^2,\sigma_c^2,R,\tau\mid\{d_s\})\\
&\quad\propto
\mathbf1_{\{\sigma_M^2,\sigma_c^2,\tau>0\}}
\prod_{s=1}^N
\left[
\frac1{\sigma_c}\exp\!\left\{-\frac{(\widetilde c_s-E_s-c_0)^2}{2\sigma_c^2}\right\}
\frac1{\sigma_M}\exp\!\left\{-\frac{[\widetilde M_s-RE_s-M_0-\beta(\widetilde c_s-E_s)]^2}{2\sigma_M^2}\right\}
\frac1\tau e^{-E_s/\tau}\mathbf1_{\{E_s\geq0\}}
\right].
\end{aligned}
$$

Its [Directed acyclic graph](../../../../../../directed-acyclic-graph.md) has, for each star, the arrows

$$
(c_0,\sigma_c^2)\to c_s,
\qquad
(M_0,\beta,\sigma_M^2,c_s)\to M_s,
\qquad
\tau\to E_s,
$$

followed by the deterministic observation arrows

$$
(c_s,E_s)\to\widetilde c_s,
\qquad
(M_s,E_s,R)\to\widetilde M_s.
$$

The [latent variables](../../../../../../latent-variable.md) $(c_s,M_s,E_s)$ are repeated inside a plate indexed by $s=1,\ldots,N$; all hyperparameters lie outside that plate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
