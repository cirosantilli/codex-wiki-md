<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An explicit construction gives [Bernstein's lethargy theorem](../../../../../../bernstein-s-lethargy-theorem.md) in the requested inequality form. Set

$$
a_0=\epsilon_0-\epsilon_1,\qquad
a_k=\epsilon_{3^{k-1}}-\epsilon_{3^k}\quad(k\ge1).
$$

Strict decrease makes every coefficient positive. Telescoping and the limit assumption give

$$
\sum_{k=0}^\infty a_k=\epsilon_0,\qquad
\sum_{k=K}^\infty a_k=\epsilon_{3^{K-1}}\quad(K\ge1).
$$

Thus

$$
f_\epsilon(x)=\sum_{k=0}^\infty a_kT_{3^k}(x)
$$

defines a [continuous function](../../../../../../continuous-function.md) by the [Weierstrass M-test](../../../../../../weierstrass-m-test.md) and the [uniform limit theorem](../../../../../../uniform-limit-theorem.md). Apply the [positive lacunary Chebyshev series](../../../../../../positive-lacunary-chebyshev-series.md) calculation. At $n=0$,

$$
E_0(f_\epsilon)=\epsilon_0.
$$

For $n\ge1$, choose $K\ge1$ so that $3^{K-1}\le n<3^K$. Its error is

$$
E_n(f_\epsilon)=\epsilon_{3^{K-1}}\ge\epsilon_n.
$$

Therefore the function satisfies

$$
\boxed{E_n(f_\epsilon)\ge\epsilon_n\quad\text{for every }n\ge0}.
$$

This [explicit Chebyshev construction for Bernstein lethargy](../../../../../../explicit-chebyshev-construction-for-bernstein-lethargy.md) also has $E_n(f_\epsilon)\to0$. It shows that continuity imposes no universal speed of convergence of best [polynomial](../../../../../../polynomial-split.md) approximation, even though convergence itself follows from the [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
