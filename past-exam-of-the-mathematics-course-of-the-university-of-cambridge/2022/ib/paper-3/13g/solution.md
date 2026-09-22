<h1 id="13g/solution">Solution</h1>

↑ **Parent:** [13G](../13g.md)

Uniform convergence on compact subsets makes $f$ continuous. For every triangle whose closure lies in $U$, uniform convergence on its boundary permits passage through the contour integral:

$$
\int_{\partial\Delta}f(z),dz
=\lim_{n\to\infty}\int_{\partial\Delta}f_n(z),dz=0.
$$

[Morera's theorem](../../../../../morera-s-theorem.md) implies that $f$ is holomorphic. If a compact set $K\Subset U$ is surrounded by a finite union of contours at positive distance from $K$, the [Cauchy integral formula for derivatives](../../../../../cauchy-derivative-formula.md) gives

$$
f_n'(z)-f'(z)
=\frac1{2\pi i}\int_\Gamma
\frac{f_n(\zeta)-f(\zeta)}{(\zeta-z)^2},d\zeta.
$$

The uniform bound on the surrounding compact set proves that $f_n'\to f'$ uniformly on $K$.

If $f$ had distinct zeros $c$ and $d$, choose disjoint small closed discs around them whose boundary contains no zero of $f$. Uniform convergence and [Rouché's theorem](../../../../../rouche-s-theorem.md) imply that, for large $n$, $f_n$ has a zero in each disc, contradicting uniqueness of $c_n$. Thus $f$ has at most one zero.

For an example on the unit disc, take

$$
f_n(z)=z-(1-1/n),
\qquad c_n=1-1/n.
$$

Then $f_n\to f(z)=z-1$, which has no zero in the open disc. In general, [Hurwitz's theorem](../../../../../hurwitz-s-theorem.md) shows that $f$ is zero-free exactly when the unique zeros escape every compact subset of $U$:

$$
\boxed{
\text{for every compact }K\Subset U,
\quad c_n\notin K\text{ eventually}.}
$$

Indeed, an interior accumulation point of $c_n$ is a zero of $f$, while a zero of $f$ forces the unique $c_n$ into each of its sufficiently small neighbourhoods.

## ↑ Ancestors (10)

1. [13G](../13g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
