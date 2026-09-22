<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $\Re s>1$, the [Dirichlet series](../../../../../../dirichlet-series.md) multiplication rule and $-\zeta'/\zeta(s)=\sum_{n\geq1}\Lambda(n)n^{-s}$ give

$$
\left(\frac{\zeta'(s)}{\zeta(s)}\right)^2
=\sum_{n=1}^{\infty}\frac{(\Lambda*\Lambda)(n)}{n^s}.
$$

Apply an effective [Perron formula](../../../../../../perron-s-formula.md) on the line $\kappa=1+1/\log x$ and truncate at

$$
T=\exp(\sqrt{\log x}).
$$

The bound from part (c) controls the truncation error.

Use the classical [zero-free region of the Riemann zeta function](../../../../../../zero-free-region-of-the-riemann-zeta-function.md)

$$
\zeta(s)\ne0
\quad\text{when}\quad
\Re s\geq1-\frac{c_0}{\log(|\Im s|+3)},
$$

together with $\zeta'/\zeta(s)\ll\log^2(|\Im s|+3)$ there. [Contour shifting](../../../../../../contour-shifting.md) moves the Perron contour to $\Re s=1-c_1/\log T$. The only crossed singularity is the double pole at $s=1$, whose [residue](../../../../../../residue.md) is $x\log x+Ax$ by part (b). On the new contour,

$$
|x^s|
\leq x\exp\left(-\frac{c_1\log x}{\log T}\right)
=x\exp(-c_1\sqrt{\log x}),
$$

and the logarithmic-derivative bounds contribute only powers of $\log x$, which can be absorbed by reducing the positive constant in the exponential. The horizontal integrals and Perron truncation error are $O(x\exp(-c_2\sqrt{\log x}))$ as well. Therefore, for some $c>0$,

$$
\boxed{\sum_{n\leq x}(\Lambda*\Lambda)(n)
=x\log x+Ax+O\bigl(x\exp(-c\sqrt{\log x})\bigr).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
