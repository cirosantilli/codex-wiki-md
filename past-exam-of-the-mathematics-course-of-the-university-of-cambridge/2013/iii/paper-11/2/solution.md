<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $e(t)=\exp(2\pi it)$. A sequence in the [circle group](../../../../../circle-group.md) is an [equidistributed sequence](../../../../../equidistributed-sequence.md) if, for every interval $I\subseteq\mathbb R/\mathbb Z$,

$$
\frac1N\#\{1\leq n\leq N:\phi(n)\in I\}\longrightarrow |I|,
$$

where $|I|$ is its normalized length. Equivalently, averages of every continuous function along the sequence tend to its circle integral. [Trigonometric polynomials](../../../../../trigonometric-polynomial.md) approximate continuous functions, and interval indicators can be squeezed between continuous functions with arbitrarily close integrals. The nonconstant [additive characters](../../../../../additive-character.md) have integral zero. These facts give the [Weyl criterion](../../../../../weyl-criterion.md):

$$
\boxed{\phi\text{ is equidistributed}\iff\mathbb E_{n\leq N}e(m\phi(n))\to0\quad\text{for every }m\in\mathbb Z\setminus\{0\}.}
$$

This is the link between [equidistribution](../../../../../equidistributed-sequence.md) and cancellation in [exponential sums](../../../../../exponential-sum.md).

Suppose every positive-shift difference sequence were equidistributed. Fix $m\ne0$ and set $z_n=e(m\phi(n))$. For every fixed $h\geq1$, the [Weyl criterion](../../../../../weyl-criterion.md) would give

$$
\frac1N\sum_{n=1}^{N-h}z_n\overline{z_{n+h}}\to0.
$$

The omitted final $h$ terms change a normalized average by at most $h/N$.

Here is the needed [Van der Corput inequality for finite scalar sequences](../../../../../van-der-corput-inequality-for-finite-scalar-sequences.md). Extend $z_n$ by zero outside $[1,N]$ and average $H$ consecutive translates of the sum. [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) gives

$$
\left|\frac1N\sum_{n=1}^Nz_n\right|^2
\leq\frac{N+H-1}{N}\left[\frac1H+\frac2{H^2}\sum_{h=1}^{H-1}(H-h)\operatorname{Re}\left(\frac1N\sum_{n=1}^{N-h}z_n\overline{z_{n+h}}\right)\right].
$$

Indeed, apply [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) to $H\sum_nz_n=\sum_t\sum_{j=0}^{H-1}z_{t-j}$ and expand the squared inner sum. Taking $N\to\infty$ first leaves a bound $1/H$; then let $H\to\infty$. Every nonzero Fourier average of $\phi$ vanishes, so the [Weyl criterion](../../../../../weyl-criterion.md) makes $\phi$ equidistributed. This is the [differencing obstruction to equidistribution](../../../../../differencing-obstruction-to-equidistribution.md). By contraposition, **a non-equidistributed sequence has a non-equidistributed difference for some positive $h$**, hence for some $h\ne0$ as requested.

For $\phi(n)=\sqrt2\,n^2$, the difference is $\Delta_h\phi(n)=-2h\sqrt2\,n-h^2\sqrt2$. For any nonzero integer $m$, its [exponential sum](../../../../../exponential-sum.md) is a constant phase times a [geometric progression](../../../../../geometric-progression.md) with ratio $e(-2mh\sqrt2)\ne1$. Its normalized magnitude is at most $2/(N|1-e(-2mh\sqrt2)|)$, which tends to zero. Thus every positive-shift difference is equidistributed, and the contraposition just established proves

$$
\boxed{(\sqrt2\,n^2)_{n\geq1}\text{ is equidistributed in }\mathbb R/\mathbb Z.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
