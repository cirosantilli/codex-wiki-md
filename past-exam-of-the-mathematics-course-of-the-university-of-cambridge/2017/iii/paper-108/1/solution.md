<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A continuous transformation $T$ of a compact [metric space](../../../../../metric-space.md) $X$ is [uniquely ergodic](../../../../../unique-ergodicity.md) when there is exactly one $T$-invariant [Borel probability measure](../../../../../borel-probability-measure.md) on $X$. We use the usual compact-space convention for [unique ergodicity](../../../../../unique-ergodicity.md); the compactness and continuity hypotheses matter in the assertion about all starting points.

Let $R_\alpha(x)=x+\alpha\pmod1$ on the [circle group](../../../../../circle-group.md), with $\alpha$ irrational. Normalized [Lebesgue measure](../../../../../lebesgue-measure.md) $m$ is invariant under this [irrational rotation of the circle](../../../../../irrational-rotation.md). If $\nu$ is any invariant [Borel probability measure](../../../../../borel-probability-measure.md), define its [Fourier coefficients](../../../../../fourier-coefficient.md) by $c_k=\int e^{2\pi ikx}\,d\nu(x)$. Invariance gives

$$
c_k=\int e^{2\pi ikR_\alpha(x)}\,d\nu(x)=e^{2\pi ik\alpha}c_k.
$$

For $k\ne0$, irrationality makes $e^{2\pi ik\alpha}\ne1$, so $c_k=0$; also $c_0=1$. These are the [Fourier coefficients](../../../../../fourier-coefficient.md) of $m$. Hence $\nu$ and $m$ have the same integrals against every [trigonometric polynomial](../../../../../trigonometric-polynomial.md). Such polynomials are uniformly dense in the continuous functions by the [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md), so the measures agree on every continuous test function and therefore agree as [Borel measures](../../../../../borel-measure.md). Thus

$$
\boxed{R_\alpha\text{ is uniquely ergodic, with invariant measure }m}.
$$

For the general [uniquely ergodic](../../../../../unique-ergodicity.md) system, fix $x\in X$ and form the [empirical measures](../../../../../empirical-measure.md)

$$
\nu_{N,x}=\frac1N\sum_{n=0}^{N-1}\delta_{T^nx}.
$$

On a compact [metric space](../../../../../metric-space.md), the [Borel probability measures](../../../../../borel-probability-measure.md) are compact for [weak convergence of probability measures](../../../../../weak-convergence-of-probability-measures.md). Any subsequential limit $\nu$ is invariant: for every continuous $g$,

$$
\int(g\circ T-g)\,d\nu_{N,x}=\frac{g(T^Nx)-g(x)}N\longrightarrow0.
$$

Here $g$ is bounded and $g\circ T$ is continuous, so the identity passes to the limit. Uniqueness of the invariant [Borel probability measure](../../../../../borel-probability-measure.md) gives $\nu=\mu$. Every subsequential limit is therefore $\mu$, and compactness implies convergence of the entire sequence. Testing against $f$ proves

$$
\boxed{\lim_{N\to\infty}\frac1N\sum_{n=0}^{N-1}f(T^nx)=\int f\,d\mu\quad\text{for every }x\in X}.
$$

In fact this proves [uniform ergodic convergence for uniquely ergodic systems](../../../../../uniform-ergodic-convergence-for-uniquely-ergodic-systems.md): if convergence were not uniform in $x$, choose $N_j\to\infty$ and $x_j$ where the discrepancy stays above a fixed positive number. The same compactness and telescoping argument applied to $\nu_{N_j,x_j}$ forces a subsequence to converge to $\mu$, a contradiction. This also makes clear why an almost-everywhere [Birkhoff ergodic theorem](../../../../../birkhoff-ergodic-theorem.md) alone would not establish the requested everywhere assertion. Without the compact-space hypothesis the assertion need not hold: on the discrete space $\{p\}\sqcup\mathbb Z_{\ge0}$, set $T(p)=p$ and $T(n)=n+1$. The only invariant probability is $\delta_p$, but the continuous bounded function which is zero at $p$ and one on the integer orbit has orbit average one there.

For the decimal application put $\alpha=\log_{10}2$. This is irrational: if $\alpha=p/q$ with positive integers $p,q$, then $2^q=10^p=2^p5^p$, contradicting [unique prime factorization](../../../../../fundamental-theorem-of-arithmetic.md). Writing $n\alpha=m_n+t_n$ with $m_n=\lfloor n\alpha\rfloor$ and $t_n\in[0,1)$ gives $2^n=10^{m_n}10^{t_n}$. Its leading decimal digit is seven exactly when

$$
t_n\in I=[\log_{10}7,\log_{10}8).
$$

The half-open upper endpoint correctly excludes powers whose leading digit is eight, including $2^3=8$.

The indicator of $I$ is not continuous, so an extra step is needed. For any $\varepsilon>0$, choose continuous functions $a_\varepsilon,b_\varepsilon$ on the circle with $0\le a_\varepsilon\le\mathbf1_I\le b_\varepsilon\le1$ and $\int(b_\varepsilon-a_\varepsilon)\,dm<\varepsilon$, by tapering in small neighbourhoods of the two endpoints. Applying the everywhere averaging result to these functions traps the lower and upper limits of the interval frequency between their integrals. Letting $\varepsilon\downarrow0$ proves [everywhere interval frequency under an irrational rotation](../../../../../everywhere-interval-frequency-under-an-irrational-rotation.md). Consequently

$$
\boxed{\lim_{N\to\infty}\frac{|S\cap[0,N-1]|}{N}=m(I)=\log_{10}8-\log_{10}7=\frac{\log8-\log7}{\log10}}.
$$

This is the leading-seven case of [Benford frequencies for powers of an integer](../../../../../benford-frequencies-for-powers-of-an-integer.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
