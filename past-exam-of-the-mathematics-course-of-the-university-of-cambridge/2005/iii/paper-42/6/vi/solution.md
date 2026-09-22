<h1 id="6/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Population [influence functions](../../../../../../influence-function.md) describe infinitesimal [contamination](../../../../../../contamination-statistics.md); finite-sample analogues examine actual changes to an empirical sample. For its [empirical distribution](../../../../../../type-information-theory.md) $F_n$, add an observation $z$ and define the [sensitivity curve](../../../../../../sensitivity-curve.md)

$$
\operatorname{SC}_n(z)=(n+1)\left[T\left(\frac n{n+1}F_n+\frac1{n+1}\delta_z\right)-T(F_n)\right].
$$

Under suitable differentiability it approximates the [influence function](../../../../../../influence-function.md). A replacement version is $\operatorname{RC}_{n,i}(z)=n[T_n(y_1,\ldots,z,\ldots,y_n)-T_n(y)]$, approximately $\operatorname{IF}(z;T,F_n)-\operatorname{IF}(y_i;T,F_n)$. Their supremum magnitudes quantify finite one-observation sensitivity.

The [empirical influence function](../../../../../../empirical-influence-function.md) instead substitutes $F_n$ directly in $\operatorname{IF}(z;T,F)$. For a differentiable [M-estimator](../../../../../../m-estimator.md) this gives $-\psi(z,T(F_n))/[n^{-1}\sum_i\partial_\theta\psi(y_i,T(F_n))]$. For quantile functionals, a discrete unsmoothed empirical law may not admit the required density derivative; a [sensitivity curve](../../../../../../sensitivity-curve.md) or a smoothed empirical law is then preferable.

Global contamination is measured by [finite-sample maximum bias](../../../../../../finite-sample-maximum-bias.md) $b_n(m;y)=\sup_{z:d_H(z,y)\leq m}|T_n(z)-T_n(y)|$, where $d_H$ counts replacements. Under the convention of the first fraction that causes unbounded bias,

$$
\boxed{\varepsilon_n^*(T;y)=\frac1n\min\{m:b_n(m;y)=\infty\}.}
$$

This is the finite-sample [replacement breakdown point](../../../../../../replacement-breakdown-point.md). The largest replacement fraction still guaranteed bounded is one grid step smaller, so the conventions must be specified. One replacement sends a [sample mean](../../../../../../sample-mean.md) arbitrarily far, giving $1/n$, while the ordinary scalar [sample median](../../../../../../sample-median.md) has first-breaking fraction $\lceil n/2\rceil/n$ with the usual midpoint convention for even samples. Its limiting value is $1/2$. Local influence and global breakdown answer different questions; a bounded [influence function](../../../../../../influence-function.md) is not by itself a proof of a high breakdown point.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [6](../../6.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
