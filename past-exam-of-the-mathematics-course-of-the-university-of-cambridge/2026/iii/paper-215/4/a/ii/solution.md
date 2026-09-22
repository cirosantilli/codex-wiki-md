<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $D=\max_{x,y}\rho(x,y)$ and let $\pi$ be the invariant distribution. Iterating the assumed [Wasserstein contraction](../../../../../../../wasserstein-contraction.md) gives

$$
\rho_K(P^t(x,\cdot),\pi)
=\rho_K(P^t(x,\cdot),\pi P^t)
\leq e^{-\alpha t}\rho_K(\delta_x,\pi)
\leq e^{-\alpha t}D.
$$

Since $\rho(x,y)\geq\mathbf1_{\{x\ne y\}}$, the [coupling characterization of total variation distance](../../../../../../../coupling-characterization-of-total-variation-distance.md) implies

$$
\lVert P^t(x,\cdot)-\pi\rVert_{\mathrm{TV}}
\leq\rho_K(P^t(x,\cdot),\pi)
\leq e^{-\alpha t}D.
$$

The right side is at most $\varepsilon$ when

$$
t\geq\frac1\alpha(\log D-\log\varepsilon),
$$

which proves the claimed mixing bound.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 215](../../../../paper-215-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
