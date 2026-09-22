<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat m(t)=\int e^{-itx}\,dm(x)$. The [complex measure](../../../../../complex-measure.md) is finite because $\sum_n|f(n)|n^{-\sigma}<\infty$. The [Möbius divisor-sum identity](../../../../../mobius-divisor-sum-identity.md), proved in the preceding solution, allows multiplication of absolutely convergent [Dirichlet series](../../../../../dirichlet-series.md) and gives

$$
F(s):=\sum_{n\ge1}\mu(n)n^{-s}=\frac1{\zeta(s)},\qquad \Re s>1.
$$

Here $\zeta$ is the [Riemann zeta function](../../../../../riemann-zeta-function.md). We prove the estimates in the intended range $1<\sigma\le2$. A uniform estimate of the printed form for all $\sigma>1$ would be false: at $t=0$, $F(\sigma)\to1$ as $\sigma\to\infty$, while its proposed upper bound tends to zero. A version valid for every $\sigma>1$ replaces $(\sigma-1)^{-3/4}$ by $1+(\sigma-1)^{-3/4}$.

For completeness, [unique prime factorization](../../../../../fundamental-theorem-of-arithmetic.md) and absolute convergence give $\zeta(s)=\prod_p(1-p^{-s})^{-1}$ and

$$
\log\zeta(s)=\sum_p\sum_{m\ge1}\frac{p^{-ms}}m
$$

as the logarithm defined by that [Euler product](../../../../../euler-product.md). The elementary nonnegative [trigonometric polynomial](../../../../../trigonometric-polynomial.md)

$$
3+4\cos v+\cos(2v)=2(1+\cos v)^2
$$

therefore proves the [three-four-one inequality for Euler products](../../../../../three-four-one-inequality-for-euler-products.md)

$$
\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\ge1.
$$

We also need elementary uniform bounds for [derivatives](../../../../../derivative.md) of the [Riemann zeta function](../../../../../riemann-zeta-function.md). For an integer $H\ge1$, summation by parts gives

$$
\zeta(s)=\sum_{n\le H}n^{-s}
+\frac{H^{1-s}}{s-1}
-s\int_H^\infty\{u\}u^{-s-1}\,du.
$$

This continues the function to $\Re s>0$ with just the pole at one. For $1\le\sigma\le2$, $|t|\ge1$, choose $H=\lceil2+|t|\rceil$. Differentiating $j$ times, the finite [Dirichlet polynomial](../../../../../dirichlet-polynomial.md) is bounded by $\sum_{n\le H}(\log n)^j/n\ll_j\log^{j+1}(2+|t|)$. Derivatives of the second term have the same bound, since $|s-1|\ge1$. In the last term, differentiated integrands are bounded by $u^{-\sigma-1}(\log u)^j$, whose integral is $O_j(H^{-\sigma}\log^j(2H))$; multiplication by $|s|\ll H$ is harmless. It follows that

$$
\zeta^{(j)}(\sigma+it)\ll_j\log^{j+1}(2+|t|).
$$

As $\zeta(\sigma)\le1+(\sigma-1)^{-1}$, the [three-four-one inequality for Euler products](../../../../../three-four-one-inequality-for-euler-products.md) gives, for $|t|\ge1$,

$$
|F(\sigma+it)|\ll(\sigma-1)^{-3/4}\log^{1/4}(2+|t|).
$$

To handle bounded $t$, first note that $\zeta$ cannot vanish at $1+it_0$ for $t_0\ne0$: a zero of order $m\ge1$ would make the three-four-one product $O((\sigma-1)^{4m-3})\to0$, contradicting its lower bound one. At $s=1$, the reciprocal $F$ extends holomorphically with a simple zero, since the pole of $\zeta$ has residue one. Thus $F$ and all its [derivatives](../../../../../derivative.md) are bounded on the compact rectangle $1\le\sigma\le2$, $|t|\le1$. This proves the requested [reciprocal zeta bounds near the line one](../../../../../reciprocal-zeta-bounds-near-the-line-one.md):

$$
\boxed{|\widehat m_{\mu,\sigma}(t)|\ll(\sigma-1)^{-3/4}\log^{1/2}(2+|t|).}
$$

For the derivative estimate, repeatedly differentiate $F=1/\zeta$. Every term of $F^{(k)}$ is a constant times

$$
\frac{\prod_{j=1}^k(\zeta^{(j)})^{m_j}}{\zeta^{r+1}},
\qquad \sum_j j m_j=k,\quad r=\sum_jm_j\le k.
$$

The preceding [derivative](../../../../../derivative.md) bounds and reciprocal estimate bound this by $O_k((\sigma-1)^{-3(k+1)/4}\log^{3k+1}(2+|t|))$. Compact-height bounds supply the remaining range. Since $\partial_t^kF(\sigma+it)=i^kF^{(k)}(\sigma+it)$, this has exactly the requested dependence, with an explicit logarithmic exponent linear in $k$ for $k\ge1$.

Here is the [unsmoothing a logarithmically weighted sum](../../../../../unsmoothing-a-logarithmically-weighted-sum.md) argument with the normalization repaired. For real $v$,

$$
\frac1{2\pi}\int_{\mathbb R}\frac{e^{v(\sigma+it)}}{(\sigma+it)^2}\,dt=v_+.
$$

Indeed the [Fourier transform](../../../../../fourier-transform.md) of $u e^{-\sigma u}\mathbf1_{u\ge0}$ is $(\sigma+it)^{-2}$, so [Fourier inversion](../../../../../fourier-inversion-theorem.md) gives the identity, also at $v=0$ by continuity. In a vertical contour integral the coefficient is $1/(2\pi i)$ and the differential is $ds=i\,dt$. The printed real-$t$ integral has $dt$ with $1/(2\pi i)$ and is missing this factor of $i$.

Set $a_m=\mu(m)(\log m)^k$, taking $(\log1)^0=1$ when $k=0$. Its [Dirichlet series](../../../../../dirichlet-series.md) is $(-1)^kF^{(k)}(s)$. The [logarithmically smoothed Perron formula](../../../../../logarithmically-smoothed-perron-formula.md), justified by absolute convergence, gives

$$
A_k(x):=\sum_{m\le x}a_m\log(x/m)
=\frac1{2\pi}\int_{\mathbb R}
\frac{(-1)^kF^{(k)}(\sigma+it)x^{\sigma+it}}{(\sigma+it)^2}\,dt.
$$

For $x\ge3$ choose $\sigma=1+1/\log x$. The integral of $\log^{3k+1}(2+|t|)/|\sigma+it|^2$ is finite, with a constant depending only on $k$, and $x^\sigma=ex$. Thus, with $\beta=3(k+1)/4$,

$$
A_k(x)=O_k(x(\log x)^\beta).
$$

For $0<h\le1$, subtraction gives the exact finite-difference identity

$$
A_k(xe^h)-A_k(x)
=h\sum_{m\le x}a_m
+\sum_{x<m\le xe^h}a_m\log(xe^h/m).
$$

The last sum is $O_k((xh^2+h)(\log x)^k)$, since there are $O(xh+1)$ terms. Consequently

$$
\left|\sum_{m\le x}a_m\right|
\ll_k xh^{-1}(\log x)^\beta+xh(\log x)^k+(\log x)^k.
$$

For $k\ge3$, choose $h=(\log x)^{(\beta-k)/2}$ to get exponent $(\beta+k)/2=7k/8+3/8$. For $0\le k<3$, the trivial bound $O_k(x(\log x)^k)$ is already no larger than that estimate. The extra $(\log x)^k$ term is absorbed for fixed $k$. Hence

$$
\boxed{\sum_{m\le x}\mu(m)(\log m)^k
=O_k\left(x(\log x)^{7k/8+3/8}\right),\qquad c=\frac18.}
$$

This also yields the cancellation needed for the [Prime number theorem](../../../../../prime-number-theorem.md). Choose a fixed $k>3$, discard $m\le\sqrt x$ at cost $O(\sqrt x)$ for the unweighted sum, and use [partial summation](../../../../../abel-s-summation-formula.md) with $(\log m)^{-k}$ on the rest. The displayed bound gives $M(x)=O_k(x(\log x)^{-k/8+3/8})=o(x)$; the preceding solution then gives $\psi(x)\sim x$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
