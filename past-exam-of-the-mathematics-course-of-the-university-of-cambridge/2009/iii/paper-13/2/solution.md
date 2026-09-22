<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $e(t)=e^{2\pi it}$. We first prove the needed cancellation of [quadratic exponential sums](../../../../../quadratic-exponential-sum.md), rather than invoke [equidistribution](../../../../../equidistributed-sequence.md) without proof. The number $\sqrt2$ is irrational: writing it as a reduced fraction would make its numerator even from $u^2=2v^2$, and then its denominator even as well, a contradiction. Thus $2hr\sqrt2$ is irrational for nonzero [integers](../../../../../integer.md) $h,r$.

Fix $h\ne0$ and set $z_n=e(h\sqrt2\,n^2)$ for $1\leq n\leq L$, extending it by zero otherwise. For [integers](../../../../../integer.md) $L\geq H\geq1$, each term appears exactly $H$ times in the shifted sum, so

$$
H\sum_{n=1}^Lz_n=\sum_{n=1}^{L+H-1}\sum_{j=0}^{H-1}z_{n-j}.
$$

For any complex numbers $w_1,\ldots,w_J$, nonnegativity of $\sum_j|w_j-J^{-1}\sum_iw_i|^2$ gives $|\sum_jw_j|^2\leq J\sum_j|w_j|^2$. Apply this special [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) to the displayed outer sum, and then expand the inner squared modulus. This gives

$$
\left|\sum_{n=1}^Lz_n\right|^2
\leq\frac{L+H-1}{H^2}\left[HL+2\sum_{r=1}^{H-1}(H-r)\left|\sum_{n=1}^{L-r}z_{n+r}\overline{z_n}\right|\right].
$$

For fixed $H$ and large $L$, each correlation is the [geometric series](../../../../../geometric-series.md)

$$
e(hr^2\sqrt2)\sum_{n=1}^{L-r}e(2hr\sqrt2\,n),
$$

whose absolute value is at most $2/|1-e(2hr\sqrt2)|$, independently of $L$. This follows by multiplying the geometric sum by $1-e(2hr\sqrt2)$; its denominator is nonzero by irrationality. Divide the inequality by $L^2$ and let $L\to\infty$, keeping $H$ fixed. It gives a limit superior at most $1/H$. Taking arbitrarily large $H$ proves

$$
\lim_{L\to\infty}\frac1L\sum_{n=1}^Le(h\sqrt2\,n^2)=0\qquad(h\ne0).
$$

This is the quadratic instance of the [Van der Corput inequality for finite scalar sequences](../../../../../van-der-corput-inequality-for-finite-scalar-sequences.md), with its proof supplied here.

To turn cancellation into the particular approximation, put $\varepsilon=10^{-8}$ and choose an [integer](../../../../../integer.md) $M>2/\sin^2(\pi\varepsilon)$. The [Fejér kernel](../../../../../fejer-kernel.md) is the explicit finite [trigonometric polynomial](../../../../../trigonometric-polynomial.md)

$$
F_M(t)=\frac1M\left|\sum_{j=0}^{M-1}e(jt)\right|^2
=\sum_{|h|<M}\left(1-\frac{|h|}{M}\right)e(ht).
$$

The expansion follows by counting pairs of indices with difference $h$. Its constant coefficient is one, so the cancellation just proved gives

$$
\frac1L\sum_{n=1}^LF_M(n^2\sqrt2)\longrightarrow1.
$$

If $\|t\|_{\mathbb R/\mathbb Z}\geq\varepsilon$, the geometric-series formula gives

$$
F_M(t)=\frac{\sin^2(\pi Mt)}{M\sin^2(\pi t)}
\leq\frac1{M\sin^2(\pi\varepsilon)}<\frac12.
$$

For all sufficiently large $L$, the displayed average exceeds $1/2$. Consequently at least one $n\in\{1,\ldots,L\}$ satisfies

$$
\boxed{\|n^2\sqrt2\|_{\mathbb R/\mathbb Z}<10^{-8}.}
$$

It is a positive [integer](../../../../../integer.md), as required. Every auxiliary cancellation and kernel identity used in this existence proof has been derived; a smooth cutoff or an unproved [Weyl criterion](../../../../../weyl-criterion.md) is unnecessary.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
