<h1 id="33a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose the $z$-axis along $\mathbf E$, so the perturbation is

$$
\Delta H=e|\mathbf E|z
$$

up to an irrelevant sign convention for the electron charge. By [second-order nondegenerate perturbation theory](../../../../../../second-order-nondegenerate-perturbation-theory.md),

$$
E_{100}^{(2)}
=e^2|\mathbf E|^2
\sum_{\alpha\ne100}
\frac{|\langle\alpha|z|1,0,0\rangle|^2}
{E_1-E_\alpha}.
$$

Parts (a) and (b) restrict the contributing bound states to

$$
|n,1,0\rangle,\qquad n\geq2.
$$

For hydrogen,

$$
E_n=-\frac R{n^2},
$$

and hence

$$
\frac1{E_1-E_n}
=\frac1{-R+R/n^2}
=\frac1R\frac{n^2}{1-n^2}.
$$

Therefore

$$
\boxed{
E_{100}^{(2)}
=\frac{e^2|\mathbf E|^2}{R}
\sum_{n=2}^{\infty}
\frac{n^2}{1-n^2}
|\langle n,1,0|z|1,0,0\rangle|^2
}.
$$

Every denominator is negative, so the discrete-state contribution lowers the ground-state energy.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [33A](../../33a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
