<h1 id="23h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Beppo Levi theorem](../../../../../../monotone-convergence-theorem.md), or [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md), states that if $(f_n)$ is a sequence of nonnegative measurable functions on a [measure space](../../../../../../measure-space.md) and

$$
f_n\uparrow f
$$

pointwise almost everywhere, then $f$ is measurable and

$$
\boxed{\int f\,d\mu
=\lim_{n\to\infty}\int f_n\,d\mu},
$$

where either side may be infinite.

Measurability of $f=\sup_nf_n$ follows from measurability of countable suprema. Since $f_n\leq f$, [monotonicity of the Lebesgue integral](../../../../../../monotonicity-of-the-lebesgue-integral.md) gives

$$
\lim_n\int f_n\,d\mu\leq\int f\,d\mu.
$$

For the reverse inequality, let $s$ be a nonnegative [simple function](../../../../../../simple-function.md) with $s\leq f$, and fix $0<c<1$. Define

$$
E_n=\{x:f_n(x)\geq c,s(x)\}.
$$

Then $E_n\uparrow X$ up to the null set on which convergence fails. Since $f_n\geq c,s\mathbf1_{E_n}$,

$$
\int f_n\,d\mu
\geq c\int_{E_n}s\,d\mu
\longrightarrow c\int s\,d\mu
$$

by [continuity from below of a measure](../../../../../../continuity-from-below-of-a-measure.md), applied to the finitely many level sets of $s$. Hence $\lim_n\int f_n\geq c\int s$. Letting $c\uparrow1$ and taking the supremum over all simple $s\leq f$, as in the definition of the [Lebesgue integral](../../../../../../lebesgue-integral.md), gives the reverse inequality and proves the theorem.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [23H](../../23h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
