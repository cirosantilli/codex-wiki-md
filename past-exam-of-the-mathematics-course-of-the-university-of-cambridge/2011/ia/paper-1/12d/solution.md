<h1 id="12d/solution">Solution</h1>

↑ **Parent:** [12D](../12d.md)

The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) connects the [Riemann integral](../../../../../riemann-integral.md) with [differentiation](../../../../../differentiation.md). Its first part says that for [continuous](../../../../../continuous-function.md) $h:[a,b]\to\mathbb R$, the accumulation function $H(x)=\int_a^xh(t)\,dt$ is [continuous](../../../../../continuous-function.md) on $[a,b]$ and [differentiable](../../../../../differentiable-function.md) inside it, with

$$
\boxed{H'(x)=h(x).}
$$

To prove this, boundedness of $h$ gives $|H(y)-H(x)|\le\|h\|_\infty|y-x|$, proving [continuity](../../../../../continuous-function.md). For an interior point and a sufficiently small nonzero increment $u$,

$$
\frac{H(x+u)-H(x)}u-h(x)
=\frac1u\int_x^{x+u}(h(t)-h(x))\,dt.
$$

Its absolute value is at most $\sup_{|t-x|\le|u|}|h(t)-h(x)|$, which tends to zero by [continuity](../../../../../continuous-function.md) of $h$ at $x$. This proves the [derivative](../../../../../derivative.md) formula. The same estimate gives the appropriate one-sided endpoint [derivatives](../../../../../derivative.md).

The second part says that if $Q$ is [continuous](../../../../../continuous-function.md) on $[a,b]$, [differentiable](../../../../../differentiable-function.md) on $(a,b)$, and $Q'=h$ with $h$ [continuous](../../../../../continuous-function.md), then

$$
\boxed{\int_a^b h(t)\,dt=Q(b)-Q(a).}
$$

Indeed $(Q-H)'=0$, so the [mean value theorem](../../../../../mean-value-theorem.md) makes $Q-H$ constant, and evaluating at the endpoints proves the formula. A useful stronger version only requires $Q'$ to be [Riemann integrable](../../../../../riemann-integrable-function.md). For a partition $a=x_0<\cdots<x_N=b$, the [mean value theorem](../../../../../mean-value-theorem.md) on each subinterval provides $\xi_j\in(x_{j-1},x_j)$ such that

$$
Q(b)-Q(a)=\sum_{j=1}^NQ'(\xi_j)(x_j-x_{j-1}).
$$

As the mesh tends to zero, these tagged [Riemann sums](../../../../../riemann-sum.md) converge to $\int_a^b Q'$, proving that version too. Its integrability hypothesis must not be omitted.

**An integrable integrand need not give an everywhere [differentiable](../../../../../differentiable-function.md) accumulation function.** For a counterexample, let $f(t)=0$ for $t<1/2$ and $f(t)=1$ for $t\ge1/2$. This bounded step [function](../../../../../function-split.md) is [Riemann integrable](../../../../../riemann-integrable-function.md), but

$$
F(x)=\int_0^xf(t)\,dt=\begin{cases}0,&x\le1/2,\\x-1/2,&x\ge1/2.
\end{cases}
$$

Its left and right [derivatives](../../../../../derivative.md) at $1/2$ are zero and one. Thus **$F$ need not be [differentiable](../../../../../differentiable-function.md) at every interior point**. The first part of the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) does apply at every point where the integrand is [continuous](../../../../../continuous-function.md).

**A [derivative](../../../../../derivative.md) need not have a [Riemann integral](../../../../../riemann-integral.md).** Define on all of $\mathbb R$

$$
f(x)=\begin{cases}x^2\sin(1/x^2),&x\ne0,\\0,&x=0.
\end{cases}
$$

At zero $f(h)/h=h\sin(1/h^2)\to0$, so $f'(0)=0$; elsewhere the [product rule](../../../../../product-rule.md) and [chain rule](../../../../../chain-rule.md) give

$$
f'(x)=2x\sin(1/x^2)-\frac2x\cos(1/x^2).
$$

At $x_n=(2\pi n)^{-1/2}$, this equals $-2/x_n\to-\infty$. Hence $f'$ is unbounded on $[0,1]$, whereas a properly [Riemann integrable](../../../../../riemann-integrable-function.md) [function](../../../../../function-split.md) on a compact interval must be bounded. The requested [Riemann integral](../../../../../riemann-integral.md) therefore **need not exist**, even though $f$ is [differentiable](../../../../../differentiable-function.md) everywhere. This example is an [unbounded derivative obstruction to Riemann integrability](../../../../../unbounded-derivative-obstruction-to-riemann-integrability.md); it does not contradict the theorem's version that explicitly assumes integrability of the derivative.

## ↑ Ancestors (10)

1. [12D](../12d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
