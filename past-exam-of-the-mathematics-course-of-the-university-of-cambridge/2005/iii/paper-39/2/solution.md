<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The first limit in the PDF has a reciprocal error when $\lambda$ denotes point density. The correct [strong law for Poisson arrival times](../../../../../strong-law-for-poisson-arrival-times.md) is

$$
\boxed{Y_n/n\longrightarrow1/\lambda\quad\text{almost surely},\qquad\lambda>0.}
$$

To prove it, put $N(t)=\Pi((0,t])$. The unit-interval increments $N(j)-N(j-1)$ are [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with the [Poisson distribution](../../../../../poisson-distribution.md) of mean $\lambda$. The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives $N(m)/m\to\lambda$ along integers. For $m\le t<m+1$,

$$
\frac{N(m)}{m+1}\le\frac{N(t)}t\le\frac{N(m+1)}m,
$$

so $N(t)/t\to\lambda$ for all real $t\to\infty$. The continuous intensity gives distinct points almost surely, and local finiteness and infinitely many points give $Y_n\to\infty$. Since $N(Y_n)=n$, the same pathwise limit along $Y_n$ implies $n/Y_n\to\lambda$, proving the reciprocal limit. For instance at density $2$ the limit is $1/2$, not $2$. The printed limit would instead describe a parameter interpreted as mean interarrival time, but not the stated density.

For the [Non-homogeneous Poisson point process](../../../../../non-homogeneous-poisson-point-process.md) on $(0,1)$, every closed subinterval strictly inside $(0,1)$ has finite intensity. The intensity is non-atomic, so the process is simple and has no point at $1/2$ almost surely. Both half-intervals have infinite intensity: the density behaves as $x^{-2}$ at zero and as $(1-x)^{-1}$ at one. More explicitly, exhaust either half by finite-intensity intervals of means $m_j\to\infty$. For any fixed integer $K$,

$$
\mathbb P(\Pi(\text{half-interval})\le K)\le e^{-m_j}\sum_{i=0}^K\frac{m_j^i}{i!}\longrightarrow0.
$$

Thus there are infinitely many points on each side.

Local finiteness around $1/2$ gives a last point on its left and a first point on its right. To see the former directly, choose any left point; between it and $1/2$ there are only finitely many points, so there is a largest one. Repeat below each chosen point to label the left sequence by $X_{-1},X_{-2},\ldots$, and similarly label the right sequence by $X_0,X_1,\ldots$. No infinite sequence of points can accumulate in the interior, because a compact neighbourhood there has finite count. Consequently

$$
\boxed{X_n\to0\text{ as }n\to-\infty,\qquad X_n\to1\text{ as }n\to+\infty.}
$$

This constructs the required [two-sided order statistics of a boundary-singular Poisson process](../../../../../two-sided-order-statistics-of-a-boundary-singular-poisson-process.md).

Use its integrated intensity to find the rates. Partial fractions give

$$
\frac1{x^2(1-x)}=\frac1{x^2}+\frac1x+\frac1{1-x}.
$$

The left cumulative-intensity coordinate is

$$
L(x)=\int_x^{1/2}\frac{du}{u^2(1-u)}=\frac1x-2-\log\frac{x}{1-x},\qquad0<x<1/2.
$$

It maps the left half bijectively onto $(0,\infty)$, reversing its order. The image points form a unit-rate [Poisson process](../../../../../poisson-process.md) directly from the count definition: inverse images of disjoint parameter intervals are disjoint, and their intensity equals their parameter lengths. In particular $L(X_{-k})$ is its $k$th arrival, so the result just proved gives $L(X_{-k})/k\to1$. Also $xL(x)\to1$ as $x\downarrow0$, because $x\log x\to0$. Hence

$$
\boxed{kX_{-k}=\frac{k}{L(X_{-k})}\,X_{-k}L(X_{-k})\longrightarrow1.}
$$

This is exactly the requested negative-index limit.

For the right side, the increasing coordinate is

$$
F(x)=\int_{1/2}^x\frac{du}{u^2(1-u)}=2-\frac1x+\log\frac{x}{1-x},\qquad1/2<x<1.
$$

Its image is another unit-rate [Poisson process](../../../../../poisson-process.md); $F(X_n)$ is the $(n+1)$st arrival because the first right point has index zero. Thus $F(X_n)/(n+1)\to1$. As $x\uparrow1$,

$$
F(x)=1-\log(1-x)+o(1).
$$

Combining these facts gives the positive-index asymptotics

$$
\boxed{\frac{\log(1-X_n)}n\longrightarrow-1,\qquad(1-X_n)^{1/n}\longrightarrow e^{-1}\quad\text{almost surely}.}
$$

Equivalently $1-X_n=\exp(-n+o(n))$ almost surely. In particular $n^p(1-X_n)\to0$ for every fixed $p>0$, unlike the inverse-linear scale at the left endpoint.

There is also an exact distributional description, if desired. For $x\in(1/2,1)$, $X_n>x$ means that at most $n$ right-hand points precede $x$, so

$$
\mathbb P(X_n>x)=e^{-F(x)}\sum_{j=0}^n\frac{F(x)^j}{j!}.
$$

Thus $F(X_n)$ has the [gamma distribution](../../../../../gamma-distribution.md) with shape $n+1$ and rate one. This makes the indexing shift explicit and describes the fluctuations left unspecified by the logarithmic limit.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
