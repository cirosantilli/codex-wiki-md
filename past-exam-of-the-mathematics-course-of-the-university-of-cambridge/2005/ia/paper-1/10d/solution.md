<h1 id="10d/solution">Solution</h1>

↑ **Parent:** [10D](../10d.md)

For a bounded real function on $[a,b]$, take a partition $a=t_0<\cdots<t_m=b$. Its lower and upper [Darboux sums](../../../../../darboux-sum.md) are

$$
L(f,P)=\sum_{j=1}^m\inf_{[t_{j-1},t_j]}f\,(t_j-t_{j-1}),\qquad U(f,P)=\sum_{j=1}^m\sup_{[t_{j-1},t_j]}f\,(t_j-t_{j-1}).
$$

The function is [Riemann integrable](../../../../../riemann-integrable-function.md) when $\sup_P L(f,P)=\inf_P U(f,P)$; the common value is its [Riemann integral](../../../../../riemann-integral.md). Equivalently, for every $\varepsilon>0$ there is a partition with $U(f,P)-L(f,P)<\varepsilon$. A [continuous function](../../../../../continuous-function.md) is bounded and [Riemann integrable](../../../../../riemann-integrable-function.md) on each compact interval, so all the following integrals exist.

Set $h(x)=x^{-1}\int_0^xf(t)dt$ for $x>0$. Strict decrease gives $f(x)<f(t)<f(0)$ for $0<t<x$. Integrating, with strict inequalities because the difference is positive on interior subintervals, gives

$$
f(x)<h(x)<f(0).
$$

The [intermediate value theorem](../../../../../intermediate-value-theorem.md) produces $g(x)\in(0,x)$ with $f(g(x))=h(x)$, and strict monotonicity makes this point unique. Thus **there is exactly one such $g(x)$ in $(0,x)$**.

For the given [exponential function](../../../../../exponential-function.md), $h(x)=(1-e^{-x})/x$, so

$$
\boxed{g(x)=\log\left(\frac{x}{1-e^{-x}}\right).}
$$

The preceding strict bounds already prove $0<g(x)<x$; no limiting value at zero needs to be included in its domain.

For differentiability, a continuous strictly monotone function has a continuous inverse on its range. If it is differentiable at an interior point $t$ with $f'(t)\ne0$, the inverse is differentiable at $y=f(t)$, with derivative $1/f'(t)$. Indeed, setting $u=f^{-1}(y')$, inverse continuity gives $u\to t$ as $y'\to y$, and

$$
\frac{f^{-1}(y')-f^{-1}(y)}{y'-y}=\left(\frac{f(u)-f(t)}{u-t}\right)^{-1}\longrightarrow\frac1{f'(t)}.
$$

This one-dimensional inverse result needs no assumption that $f'$ is continuous. It is enough here that $f$ is differentiable and $f'<0$ at every positive argument.

The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) and the quotient rule give

$$
h'(x)=\frac{xf(x)-\int_0^xf(t)dt}{x^2}=\frac{f(x)-h(x)}x<0.
$$

Now $g=f^{-1}\circ h$ and $g(x)>0$, so the inverse derivative formula applies at every relevant point. The [monotone mean-value point of an integral average](../../../../../monotone-mean-value-point-of-an-integral-average.md) satisfies

$$
\boxed{g'(x)=\frac{h'(x)}{f'(g(x))}=\frac{f(x)-f(g(x))}{xf'(g(x))}>0.}
$$

Both numerator and denominator are negative. For the exponential example, this also agrees with $g'(x)=1/x-1/(e^x-1)>0$, since $e^x>1+x$ for $x>0$.

## ↑ Ancestors (10)

1. [10D](../10d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
