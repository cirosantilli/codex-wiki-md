<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Partition $N=mw$ bits into $m$ tribes of size $w$, and let the [tribes function](../../../../../../tribes-function.md) be one when some tribe consists entirely of ones. Permuting tribes and permuting bits within a tribe acts transitively on the $N$ coordinates, so this is a [transitive increasing event](../../../../../../transitive-increasing-event.md). Under independent bits of density $p$, its exact success [probability](../../../../../../probability.md) is

$$
u(p)=1-(1-p^w)^m.
$$

Choose $m=\lfloor(\log2)2^w\rfloor$. Then $u(1/2)\to1/2$, while $\log N=w\log2+O(\log w)$. For fixed $0<x<1$, its unique $x$-quantile is

$$
p_x=\left[1-(1-x)^{1/m}\right]^{1/w}.
$$

Put $a_x=-\log(1-x)$. Expanding $1-e^{-a_x/m}=a_x/m+O_x(m^{-2})$ gives

$$
\log p_x=-\log2+\frac1w\log\frac{a_x}{\log2}+o(w^{-2}),
\qquad
p_x=\frac12+\frac1{2w}\log\frac{a_x}{\log2}+O_x(w^{-2}).
$$

Thus, for fixed $0<\varepsilon<1/2$,

$$
\boxed{p_{1-\varepsilon}-p_\varepsilon
=\frac1{2w}\log\frac{\log(1/\varepsilon)}{-\log(1-\varepsilon)}+O_\varepsilon(w^{-2})
=\Theta_\varepsilon(1/\log N).}
$$

This positive window prevents an improvement to $o(1/\log N)$ in the [Friedgut-Kalai sharp threshold theorem](../../../../../../friedgut-kalai-sharp-threshold-theorem.md). Moreover, as the fixed error parameter tends to zero, the displayed logarithmic coefficient is $\log(1/\varepsilon)+\log\log(1/\varepsilon)+o(1)$, so the theorem's logarithmic error dependence is also optimal up to constants. This last comparison takes $w\to\infty$ for each fixed $\varepsilon$; the expansion is not being claimed uniformly for arbitrarily tiny $w$-dependent errors.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
