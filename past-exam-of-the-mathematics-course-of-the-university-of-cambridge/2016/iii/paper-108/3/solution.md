<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A continuous map $F$ of a [compact metric space](../../../../../compact-metric-space.md) is **[uniquely ergodic](../../../../../unique-ergodicity.md)** if it has exactly one [invariant measure](../../../../../invariant-measure.md) that is a [Borel probability measure](../../../../../borel-probability-measure.md). The uniqueness requirement ranges over all invariant [Borel probability measures](../../../../../borel-probability-measure.md).

For an [irrational rotation of the circle](../../../../../irrational-rotation.md), let $R_\alpha x=x+\alpha$ on $\mathbb T=\mathbb R/\mathbb Z$, and let $\nu$ be any invariant [Borel probability measure](../../../../../borel-probability-measure.md). For each integer $r$, set $\chi_r(x)=e^{2\pi irx}$. Invariance gives

$$
\int\chi_r\,d\nu=\int\chi_r\circ R_\alpha\,d\nu
=e^{2\pi ir\alpha}\int\chi_r\,d\nu.
$$

For $r\ne0$, irrationality forces $e^{2\pi ir\alpha}\ne1$, so the corresponding [Fourier coefficient](../../../../../fourier-coefficient.md) is zero. For $r=0$ it is one. These are exactly the [Fourier coefficients](../../../../../fourier-coefficient.md) of normalized [Lebesgue measure](../../../../../lebesgue-measure.md) $m$. By the [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md), [trigonometric polynomials](../../../../../trigonometric-polynomial.md) are uniformly dense in the continuous functions on the [circle group](../../../../../circle-group.md); hence $\nu$ and $m$ integrate every continuous function equally and are the same [Borel probability measure](../../../../../borel-probability-measure.md). Since $m$ is invariant, **the [irrational rotation of the circle](../../../../../irrational-rotation.md) is [uniquely ergodic](../../../../../unique-ergodicity.md), with unique measure $m$**.

For the [irrational skew shift](../../../../../irrational-skew-shift.md) on the two-dimensional [torus](../../../../../torus.md), write

$$
T(x,y)=(x+\alpha,y+x)\pmod1,\qquad
e_{r,s}(x,y)=e^{2\pi i(rx+sy)}\quad(r,s\in\mathbb Z).
$$

The map is invertible, with $T^{-1}(x,y)=(x-\alpha,y-x+\alpha)$ modulo one, and it preserves $m_2$ as allowed in the question. We first prove the [ergodic transformation](../../../../../ergodicity.md) property by the [invariant-function characterization of ergodicity](../../../../../invariant-function-characterization-of-ergodicity.md).

Let $F\in L^2(m_2)$ satisfy $F\circ T=F$. Its expansion in the [Fourier basis](../../../../../fourier-basis.md) is $F=\sum_{r,s}c_{r,s}e_{r,s}$ in $L^2$. Direct calculation of the [Koopman operator](../../../../../koopman-operator.md) gives

$$
e_{r,s}\circ T=e^{2\pi ir\alpha}e_{r+s,s}.
$$

Uniqueness of the [Fourier coefficients](../../../../../fourier-coefficient.md) therefore implies

$$
c_{r,s}=e^{2\pi i(r-s)\alpha}c_{r-s,s}.
$$

For $s\ne0$, the magnitudes of the [Fourier coefficients](../../../../../fourier-coefficient.md) along all distinct indices $(r+js,s)$, $j\in\mathbb Z$, are equal. By the [Bessel inequality](../../../../../bessel-s-inequality.md) they are square summable, so every such coefficient must be zero. When $s=0$, the relation becomes $c_{r,0}=e^{2\pi ir\alpha}c_{r,0}$, which forces $c_{r,0}=0$ for $r\ne0$. Only $c_{0,0}$ remains. Thus every invariant $L^2$ function is constant, and

$$
\boxed{(\mathbb T^2,\mathcal B,m_2,T)\text{ is ergodic}.}
$$

To prove [unique ergodicity](../../../../../unique-ergodicity.md), we will establish **uniform averages for every continuous function** directly. No theorem on [unique ergodicity](../../../../../unique-ergodicity.md) of [skew products](../../../../../skew-product.md) is needed. Induction on $n$, using the old first coordinate in the second coordinate of $T$, yields

$$
\boxed{T^n(x,y)=\left(x+n\alpha,\ y+nx+\frac{n(n-1)}2\alpha\right)\pmod1.}
$$

In particular, for a [Fourier basis](../../../../../fourier-basis.md) element,

$$
u_n=e_{r,s}(T^n(x,y))
=\exp\left(2\pi i\left[rx+sy+n(r\alpha+sx)+\frac{s\alpha}{2}n(n-1)\right]\right).
$$

If $s=0$ and $r\ne0$, this is a [geometric series](../../../../../geometric-series.md) in $n$, and

$$
\left|\frac1N\sum_{n=0}^{N-1}u_n\right|
\leq\frac{2}{N|1-e^{2\pi ir\alpha}|}\longrightarrow0
$$

uniformly in $(x,y)$.

For $s\ne0$, we give the finite [Van der Corput inequality for finite scalar sequences](../../../../../van-der-corput-inequality-for-finite-scalar-sequences.md) and its proof. For $|u_n|\leq1$, extend $u_n$ by zero outside $0\leq n<N$. Fix an integer $1\leq H\leq N$ and set $C_h=\sum_{n=0}^{N-h-1}u_{n+h}\overline{u_n}$. Every original summand appears $H$ times in the identity

$$
H\sum_{n=0}^{N-1}u_n=\sum_{j=0}^{N+H-2}\sum_{a=0}^{H-1}u_{j-a}.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), followed by expansion of the squared window sums, gives

$$
H^2\left|\sum_{n=0}^{N-1}u_n\right|^2
\leq(N+H-1)\left(HN+2\sum_{h=1}^{H-1}(H-h)|C_h|\right).
$$

Consequently the [Van der Corput inequality for finite scalar sequences](../../../../../van-der-corput-inequality-for-finite-scalar-sequences.md) is

$$
\boxed{\left|\frac1N\sum_{n=0}^{N-1}u_n\right|^2
\leq\frac{N+H-1}{NH}\left(1+2\sum_{h=1}^{H-1}\left(1-\frac hH\right)\frac{|C_h|}{N}\right).}
$$

The finite prefactor is important; the order of limits will be $N\to\infty$ with $H$ fixed, followed by $H\to\infty$.

For the [irrational skew shift](../../../../../irrational-skew-shift.md) character sequence above, differencing cancels the quadratic term:

$$
u_{n+h}\overline{u_n}
=\exp\left(2\pi i\left[s\alpha hn+h(r\alpha+sx)+\frac{s\alpha}2h(h-1)\right]\right).
$$

For every fixed $h\geq1$, $s\alpha h$ is irrational, so another [geometric series](../../../../../geometric-series.md) estimate gives

$$
\frac{|C_h|}{N}\leq\frac{2}{N|1-e^{2\pi is\alpha h}|}\longrightarrow0,
$$

uniformly in $(x,y)$. With fixed $H$, the [Van der Corput inequality for finite scalar sequences](../../../../../van-der-corput-inequality-for-finite-scalar-sequences.md) therefore implies

$$
\limsup_{N\to\infty}\sup_{(x,y)\in\mathbb T^2}
\left|\frac1N\sum_{n=0}^{N-1}e_{r,s}(T^n(x,y))\right|^2\leq\frac1H.
$$

Letting $H\to\infty$ proves that the averages of every nonconstant [Fourier basis](../../../../../fourier-basis.md) element converge uniformly to zero. The constant character has average one. This establishes [uniform equidistribution of an irrational skew shift](../../../../../uniform-equidistribution-of-an-irrational-skew-shift.md) on all [trigonometric polynomials](../../../../../trigonometric-polynomial.md).

The [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) makes these [trigonometric polynomials](../../../../../trigonometric-polynomial.md) uniformly dense in $C(\mathbb T^2)$. If $p$ approximates a continuous $g$ with $\|g-p\|_\infty<\varepsilon$, then

$$
\sup_z\left|\frac1N\sum_{n=0}^{N-1}g(T^nz)-\int g\,dm_2\right|
\leq2\varepsilon+\sup_z\left|\frac1N\sum_{n=0}^{N-1}p(T^nz)-\int p\,dm_2\right|.
$$

Taking $N\to\infty$ and then $\varepsilon\downarrow0$ proves uniform convergence to $\int g\,dm_2$ for every continuous $g$.

Finally, if $\nu$ is any invariant [Borel probability measure](../../../../../borel-probability-measure.md) for the [irrational skew shift](../../../../../irrational-skew-shift.md), invariance and this uniform convergence give

$$
\int g\,d\nu
=\int\frac1N\sum_{n=0}^{N-1}g\circ T^n\,d\nu
\longrightarrow\int g\,dm_2\qquad(g\in C(\mathbb T^2)).
$$

Thus $\nu=m_2$, since continuous functions determine [Borel probability measures](../../../../../borel-probability-measure.md) on a [compact metric space](../../../../../compact-metric-space.md). We conclude

$$
\boxed{T\text{ is uniquely ergodic, with unique invariant probability }m_2.}
$$

The uniform-average proof also shows that every starting point has the same limiting continuous-function averages, a stronger conclusion than the almost-everywhere assertion provided by the [pointwise ergodic theorem](../../../../../birkhoff-ergodic-theorem.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
