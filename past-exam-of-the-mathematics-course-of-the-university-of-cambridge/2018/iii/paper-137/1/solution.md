<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Mellin transform](../../../../../mellin-transform.md) is

$$
\boxed{M(f,s)=\int_0^\infty f(y)y^{s-1}\,dy,}
$$

where this integral converges. Rapid decay at infinity makes the integral over $[1,\infty)$ an entire function of $s$, but alone gives no control near zero. With the additional expansion, the integral initially converges absolutely for $\operatorname{Re}s>-\sigma_1$.

For $\operatorname{Re}s>1$, expand $(e^{\pi y}-1)^{-1}=\sum_{r\geq1}e^{-\pi ry}$. Absolute convergence justifies termwise integration, using the [Gamma integral](../../../../../gamma-integral.md), and gives the scaled [Bose integral](../../../../../bose-integral.md)

$$
\boxed{M\left(\frac1{e^{\pi y}-1},s\right)
=\sum_{r\geq1}(\pi r)^{-s}\Gamma(s)
=\pi^{-s}\Gamma(s)\zeta(s).}
$$

There is a missing hypothesis in the general continuation claim: one needs $\sigma_j\to+\infty$. The original PDF, like the TeX, only says that the sequence increases. Under the intended additional hypothesis, split the integral at one and subtract $r$ terms of the [asymptotic expansion](../../../../../asymptotic-expansion.md):

$$
M(f,s)=\int_1^\infty f(y)y^{s-1}\,dy
+\sum_{j=1}^r\frac{c_j}{s+\sigma_j}
+\int_0^1 y^{s+\sigma_{r+1}-1}g_r(y)\,dy.
$$

Continuity of $g_r$ at zero makes it bounded on $[0,1]$. The last integral is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on $\operatorname{Re}s>-\sigma_{r+1}$: on every compact subset, its integrand and all its $s$ derivatives are dominated by an integrable power of $y$ times a power of $|\log y|$. The expressions for successive $r$ agree on their common initial domain and hence everywhere they overlap by the [identity theorem](../../../../../identity-theorem.md). As $\sigma_{r+1}\to\infty$, these half-planes cover $\mathbb C$. Taking $r\geq j$ with $\sigma_{r+1}>\sigma_j$ isolates the term $c_j/(s+\sigma_j)$, while all other terms are [holomorphic](../../../../../complex-differentiability-at-a-point.md) near $-\sigma_j$. Thus the corrected claim is

$$
\boxed{\operatorname{Res}_{s=-\sigma_j}M(f,s)=c_j,
\quad\text{with no other poles, provided }\sigma_j\to\infty.}
$$

This is [meromorphic continuation of a Mellin transform from an asymptotic expansion](../../../../../meromorphic-continuation-of-a-mellin-transform-from-an-asymptotic-expansion.md).

To show why the correction matters, set $\sigma_j=1-1/j$, $c_j=2^{-j}$, and

$$
f(y)=\eta(y)\sum_{j\geq1}2^{-j}y^{1-1/j},
$$

where $\eta$ is continuous, equals one for $0<y\leq1$ and vanishes for $y\geq2$. On $[0,1]$, the remainder after division by $y^{\sigma_{r+1}}$ is a uniformly convergent series of nonnegative powers of $y$, so it extends continuously to zero with value $c_{r+1}$. Away from zero, define $g_r$ by the required remainder quotient; it is continuous on the rest of $[0,\infty)$ as well. Thus all the printed hypotheses hold. Its [Mellin transform](../../../../../mellin-transform.md) equals

$$
\sum_{j\geq1}\frac{2^{-j}}{s+1-1/j}
+\int_1^2 f(y)y^{s-1}\,dy.
$$

The series continues meromorphically on $\operatorname{Re}s>-1$ and has genuine poles at $-1+1/j$, accumulating at $-1$. A [meromorphic function](../../../../../meromorphic-function.md) on $\mathbb C$ cannot have such an accumulation of poles. This is the [accumulating asymptotic exponents obstruct Mellin continuation](../../../../../accumulating-asymptotic-exponents-obstruct-mellin-continuation.md) counterexample.

For the [Gamma function](../../../../../gamma-function.md), the [Gamma function recurrence](../../../../../gamma-function-recurrence.md) gives

$$
\Gamma(s)=\frac{\Gamma(s+j+1)}{s(s+1)\cdots(s+j)}.
$$

At $s=-j$ the numerator is $\Gamma(1)=1$ and the product of the nonzero denominator factors is $(-1)^jj!$. Therefore the [residues of the Gamma function](../../../../../residues-of-the-gamma-function.md) are

$$
\boxed{\operatorname{Res}_{s=-j}\Gamma(s)=\frac{(-1)^j}{j!}\quad(j\geq0).}
$$

The generating function of the [Bernoulli numbers](../../../../../bernoulli-number.md) gives the convergent expansion near zero

$$
\frac1{e^{\pi y}-1}=\sum_{n\geq0}\frac{B_n\pi^{n-1}}{n!}y^{n-1}.
$$

The subtraction proof above applies to this expansion, including its zero coefficients, which give no pole. At $s=1-n$, for $n\geq1$, the residue of its transform is $B_n\pi^{n-1}/n!$, while the residue of $\pi^{-s}\Gamma(s)$ is $\pi^{n-1}(-1)^{n-1}/(n-1)!$. Their quotient defines a [holomorphic](../../../../../complex-differentiability-at-a-point.md) continuation of the [Riemann zeta function](../../../../../riemann-zeta-function.md) at this point, including when the first residue is zero. Dividing gives the [Bernoulli formula for zeta values at nonpositive integers](../../../../../bernoulli-formula-for-zeta-values-at-nonpositive-integers.md):

$$
\boxed{\zeta(1-n)=\frac{(-1)^{n-1}B_n}{n}\quad(n\geq1).}
$$

In particular the generating-series convention is $B_1=-1/2$, so the formula includes $\zeta(0)=-1/2$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 137](../../paper-137-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
