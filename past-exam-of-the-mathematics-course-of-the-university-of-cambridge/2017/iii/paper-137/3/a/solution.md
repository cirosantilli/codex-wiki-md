<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The displayed definition uses [iterated Eisenstein summation in weight two](../../../../../../iterated-eisenstein-summation-in-weight-two.md): the sum in $n$ is evaluated before the sum in $m$, with the single $(0,0)$ term omitted. This order is essential. The two-dimensional lattice series does not have [absolute convergence](../../../../../../absolute-convergence.md), so arbitrary rearrangement would not be justified.

For noninteger $w$, the [cosecant partial-fraction identity](../../../../../../cosecant-partial-fraction-identity.md) is

$$
\sum_{n\in\mathbb Z}\frac1{(w+n)^2}=\pi^2\csc^2(\pi w).
$$

For completeness, apply the [residue theorem](../../../../../../residue-theorem.md) to $\pi\cot(\pi\zeta)/(\zeta-w)^2$ on squares with large half-integer sides. The [cotangent](../../../../../../cotangent.md) is bounded on the contours and the integral is $O(R^{-1})$. Its residues at the integers are $(n-w)^{-2}$ and its residue at $w$ is $-\pi^2\csc^2(\pi w)$, proving the formula. If $\operatorname{Im}w>0$, the geometric-series expression $\cot(\pi w)=-i(1+2\sum_{r\geq1}e^{2\pi irw})$, differentiated termwise, gives the [cotangent partial-fraction Fourier kernel](../../../../../../cotangent-partial-fraction-fourier-kernel.md)

$$
\pi^2\csc^2(\pi w)=-4\pi^2\sum_{r\geq1}r e^{2\pi irw}.
$$

Put $q=e^{2\pi iz}$ with $z$ in the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md). For positive $m$, this gives $-4\pi^2\sum_{r\geq1}r q^{mr}$. Negative $m$ gives the same value, by replacing $n$ with $-n$ in its inner sum. The $m=0$ row is $\sum_{n\ne0}n^{-2}=\pi^2/3$, by the [Basel problem](../../../../../../basel-problem.md). The resulting series in $m,r$ does have [absolute convergence](../../../../../../absolute-convergence.md), locally uniformly in $z$, so collecting the coefficient at $q^\ell$ is legitimate:

$$
G_2(z)=\frac{\pi^2}{3}-8\pi^2\sum_{m,r\geq1}r q^{mr}
=\frac{\pi^2}{3}-8\pi^2\sum_{\ell\geq1}\sigma_1(\ell)q^\ell.
$$

The coefficient is the [sum-of-divisors function](../../../../../../sum-of-divisors-function.md), since $r$ runs over the positive divisors of $\ell$. Thus

$$
\boxed{G_2(z)=\frac{\pi^2}{3}E_2(z).}
$$

There is no conflict with [vanishing of weight-two level-one modular forms](../../../../../../vanishing-of-weight-two-level-one-modular-forms.md): the [Eisenstein series of weight two](../../../../../../eisenstein-series-of-weight-two.md) has an anomalous transformation term, so it is not a weight-two [modular form](../../../../../../modular-form.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
