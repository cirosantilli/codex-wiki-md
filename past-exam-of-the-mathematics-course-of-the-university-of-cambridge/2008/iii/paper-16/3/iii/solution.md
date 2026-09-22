<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\eta=|A|/N$ and $g=1_A-\eta$. In the [norm](../../../../../../norm.md) convention, the [quadratic uniformity of a set](../../../../../../quadratic-uniformity-of-a-set.md) means

$$
\boxed{\|g\|_{U^3}\leq\alpha.}
$$

If uniformity is parametrized instead by $\|g\|_{U^3}^8\leq\alpha$, replace the parameter below by $\alpha^{1/8}$. We prove the genuine-progression conclusion by placing nonnegative weights on a region where wrapping and repeated entries are impossible.

First suppose $N\geq16$. Put $M=\lfloor N/16\rfloor$, $J=\{0,\ldots,M-1\}$, $t=M/N$, and let $w=1_J*1_J$ be the [normalized convolution on a finite group](../../../../../../normalized-convolution-on-a-finite-group.md). Define the weighted count

$$
\mathcal T=\mathbb E_{x,d}w(x)w(d-M)\prod_{j=0}^31_A(x+jd).
$$

Both weights are nonnegative. Their supports require $0\leq x\leq2M-2$ and $M\leq d\leq3M-2$ in the ordinary representatives. In particular $d\geq1$ and $x+3d\leq11M-8<N$. Every contributing [arithmetic progression](../../../../../../arithmetic-progression.md) is therefore a [set](../../../../../../set-split.md) of four distinct integers in $\{0,\ldots,N-1\}$, with no modular wrap.

The averages of both weights are $t^2$. The [convolution theorem on a finite group](../../../../../../convolution-theorem-on-a-finite-group.md) and the [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md) give

$$
\widehat w(r)=\widehat{1_J}(r)^2,\qquad\sum_r|\widehat w(r)|=\sum_r|\widehat{1_J}(r)|^2=t.
$$

[Translation](../../../../../../translation-geometry.md) multiplies coefficients by phases, so $w(d-M)$ has the same Fourier coefficient sum. Telescoping the product of the four indicators around $\eta^4$ produces four error terms, each with one factor $g$ and all other factors bounded by one.

To bound a weighted error, expand both weights in their finite [Fourier series](../../../../../../fourier-series-split.md). For frequencies $r,s$, the extra character is $e^{2\pi i(rx+sd)/N}$. Write it as

$$
e^{2\pi i(r-s)x/N}\,e^{2\pi is(x+d)/N},
$$

and absorb these two characters into the [functions](../../../../../../function-split.md) at slopes zero and one. Even if the balanced factor is one of those [functions](../../../../../../function-split.md), its $U^3$ [norm](../../../../../../norm.md) remains at most $\alpha$ by the character invariance proved in part (i). The cyclic bound of part (ii), with $C_0=6^{1/8}$, therefore bounds each unweighted Fourier term by $C_0\alpha$. Summing absolute coefficients costs at most $t^2$. Consequently

$$
\mathcal T\geq\eta^4t^4-4C_0\alpha t^2.
$$

Since $t\geq1/32$ and $\eta\geq\delta$, this is positive whenever $\alpha<\delta^4/(4096C_0)$. A positive count supplies the required genuine [arithmetic progression](../../../../../../arithmetic-progression.md). This is the argument that [triangular weights count genuine four-term progressions](../../../../../../triangular-weights-count-genuine-four-term-progressions.md); it avoids losing powers of $\log N$ by cutting off a sharp interval.

For completeness, treat $4\leq N<16$. If $A$ is a proper nonempty [subset](../../../../../../subset.md), then $\eta(1-\eta)\geq\delta/N$. The [norm](../../../../../../norm.md) bound from part (i) gives

$$
\|1_A-\eta\|_{U^3}\geq N^{-1/8}\sqrt{\eta(1-\eta)}\geq\sqrt\delta\,15^{-5/8}.
$$

Choose $\alpha$ below this bound as well. Then quadratic uniformity forces $A=\mathbb Z_N$, which contains $\{0,1,2,3\}$. Thus, for every $N\geq4$, a sufficient threshold is

$$
\boxed{0<\alpha<\min\left\{\frac{\delta^4}{4096\cdot6^{1/8}},\ \sqrt\delta\,15^{-5/8}\right\}.}
$$

The restriction $N\geq4$ is necessary: for $N=1,2,3$, the full group has [balanced subset indicator](../../../../../../balanced-indicator-function-of-a-finite-subset.md) zero and is quadratically uniform for every positive parameter, but no [subset](../../../../../../subset.md) has four elements. The printed conclusion needs this elementary size qualification.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
