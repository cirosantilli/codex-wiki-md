<h1 id="5k/solution">Solution</h1>

↑ **Parent:** [5K](../5k.md)

Write $Y_{gj}$ for the yield in replicate $j$ of genotype $g\in\{aa,Aa,AA\}$. Model 1 is the one-way cell-means model

$$
Y_{gj}=\mu_g+\varepsilon_{gj},
\qquad
\varepsilon_{gj}\mathrel{\overset{\mathrm{iid}}\sim}N(0,\sigma^2).
$$

Thus its three coefficients estimate the three genotype means directly.

Put $D_i=\mathbf1\{\text{count}_i\geq1\}$. Model 2 is

$$
Y_i=\beta_0+\beta_1D_i+\varepsilon_i,
\qquad
\varepsilon_i\mathrel{\overset{\mathrm{iid}}\sim}N(0,\sigma^2).
$$

It imposes $\mu_{Aa}=\mu_{AA}=\beta_0+\beta_1$ and $\mu_{aa}=\beta_0$. The reported finite-sample p-values assume independent normal errors, a common unknown variance in every genotype, fixed full-rank design [matrices](../../../../../matrix.md), and correctness of the relevant mean model. Random assignment of genotypes supports interpreting the fitted differences as treatment effects.

## ↑ Ancestors (10)

1. [5K](../5k.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
