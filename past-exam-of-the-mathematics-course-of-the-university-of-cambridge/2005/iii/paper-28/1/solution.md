<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat f(u)=\int_{\mathbb R}f(x)e^{-2\pi iux}\,dx$. A version of the [Poisson summation formula](../../../../../poisson-summation-formula.md) sufficient here is

$$
\boxed{\sum_{n\in\mathbb Z}f(n)=\sum_{m\in\mathbb Z}\widehat f(m)
\qquad(f\in\mathcal S(\mathbb R)).}
$$

Both sums converge absolutely. To prove it, form the [periodization of a Schwartz function](../../../../../periodization-of-a-schwartz-function.md) $P(x)=\sum_{n\in\mathbb Z}f(x+n)$. The rapid decay of $f$ and all its derivatives makes this series and its differentiated series uniformly convergent on $[0,1]$, so $P$ is smooth and one-periodic. Its [Fourier coefficients](../../../../../fourier-coefficient.md) are

$$
\begin{aligned}
\int_0^1P(x)e^{-2\pi imx}\,dx
&=\sum_n\int_0^1f(x+n)e^{-2\pi imx}\,dx\\
&=\int_{\mathbb R}f(y)e^{-2\pi imy}\,dy=\widehat f(m).
\end{aligned}
$$

Repeated integration by parts makes these coefficients rapidly decreasing. Thus $\sum_m\widehat f(m)e^{2\pi imx}$ converges absolutely and uniformly and has the same coefficients as $P$. By uniqueness of [Fourier series](../../../../../fourier-series-split.md) it equals $P$. Evaluation at zero proves the formula.

For $u>0$, the Gaussian $f(x)=e^{-\pi ux^2}$ has transform $u^{-1/2}e^{-\pi m^2/u}$. This follows from the [Gaussian integral](../../../../../gaussian-integral.md) at frequency zero and integration by parts, which gives the differential equation $\widehat f'(v)=-(2\pi v/u)\widehat f(v)$. Hence the [Jacobi theta function](../../../../../jacobi-theta-function.md)

$$
\Theta(u)=\sum_{n\in\mathbb Z}e^{-\pi n^2u}
$$

satisfies $\Theta(u)=u^{-1/2}\Theta(1/u)$.

Use the normalization of the [completed Riemann zeta function](../../../../../completed-riemann-zeta-function.md)

$$
\Xi(s)=\pi^{-s/2}\Gamma(s/2)\zeta(s).
$$

Initially, for $\Re s>1$, the [Gamma function](../../../../../gamma-function.md) integral and [absolute convergence](../../../../../absolute-convergence.md) give its [Mellin transform](../../../../../mellin-transform.md) representation

$$
\Xi(s)=\frac12\int_0^\infty(\Theta(u)-1)u^{s/2-1}\,du.
$$

Indeed, the two equal terms for $n$ and $-n$ cancel the factor $1/2$, and the $n$th integral is $\pi^{-s/2}\Gamma(s/2)n^{-s}$.

Split at $u=1$ and use the theta transformation in the integral over $(0,1)$. Its elementary part is

$$
\frac12\int_0^1(u^{-1/2}-1)u^{s/2-1}\,du
=\frac1{s-1}-\frac1s.
$$

In the remaining part substitute $v=1/u$. Define

$$
J(s)=\int_1^\infty(\Theta(u)-1)u^{s/2-1}\,du.
$$

The [pole-subtracted theta integral for the completed zeta function](../../../../../pole-subtracted-theta-integral-for-the-completed-zeta-function.md) is therefore

$$
\boxed{\Xi(s)=\frac1{s-1}-\frac1s+\frac12\bigl(J(s)+J(1-s)\bigr).}
$$

Since $\Theta(u)-1=O(e^{-\pi u})$ for $u\geq1$, both integrals and every derivative in $s$ converge uniformly on compact subsets of $\mathbb C$. Thus $J$ is an [entire function](../../../../../entire-function.md). The boxed identity supplies the [meromorphic continuation](../../../../../meromorphic-continuation.md) of $\Xi$ to the whole plane, with no other singularities. Its [poles](../../../../../pole.md) really are simple, because the residues of the displayed rational terms are nonzero:

$$
\boxed{\operatorname{Res}_{s=0}\Xi=-1,\qquad
\operatorname{Res}_{s=1}\Xi=1.}
$$

The identity also gives $\Xi(s)=\Xi(1-s)$, the completed [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
