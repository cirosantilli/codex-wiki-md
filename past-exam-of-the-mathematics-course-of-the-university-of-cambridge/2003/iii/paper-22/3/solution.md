<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [Jacobi theta function](../../../../../jacobi-theta-function.md) $\Theta(t)=\sum_{n\in\mathbb Z}e^{-\pi n^2t}$, $t>0$. Its transformation law follows directly from the [Gaussian Fourier transform](../../../../../fourier-transform-of-a-gaussian.md). With the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat f(\xi)=\int_{\mathbb R}f(u)e^{-2\pi i\xi u}\,du$,

$$
\widehat{e^{-\pi t u^2}}(\xi)=t^{-1/2}e^{-\pi\xi^2/t}.
$$

For example, differentiating the transform and using [integration by parts](../../../../../integration-by-parts.md) gives $\widehat f'(\xi)=-(2\pi\xi/t)\widehat f(\xi)$; its value at zero is the [Gaussian integral](../../../../../gaussian-integral.md) $t^{-1/2}$. Periodize the Gaussian. Its [Fourier coefficients](../../../../../fourier-coefficient.md) are these transforms at [integer](../../../../../integer.md) frequencies, and both series converge absolutely, so evaluating its [Fourier series](../../../../../fourier-series-split.md) at zero proves the [Poisson summation formula](../../../../../poisson-summation-formula.md) here:

$$
\Theta(t)=t^{-1/2}\Theta(1/t).
$$

For $\Re s>1$, integrating the exponentially convergent series termwise gives the [Mellin representation of the completed Riemann zeta function](../../../../../mellin-representation-of-the-completed-riemann-zeta-function.md)

$$
\Lambda(s):=\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\frac12\int_0^\infty(\Theta(t)-1)t^{s/2-1}\,dt.
$$

Split at one and substitute $u=1/t$ in the lower part, using the transformation just proved. The contribution of $t^{-1/2}-1$ is $1/(s-1)-1/s$. We obtain the [pole-subtracted theta integral for the completed zeta function](../../../../../pole-subtracted-theta-integral-for-the-completed-zeta-function.md)

$$
\Lambda(s)=\frac1{s-1}-\frac1s
+\frac12\int_1^\infty(\Theta(t)-1)
\left(t^{s/2-1}+t^{(1-s)/2-1}\right)\,dt.
$$

The integral is [entire](../../../../../entire-function.md): $\Theta(t)-1$ decays exponentially, uniformly dominating the integrand and all its $s$ derivatives on [compact sets](../../../../../compact-space.md). Both the rational term and the integral are invariant under $s\mapsto1-s$. This proves the meromorphic identity

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s).}
$$

Equivalently the [Riemann xi function](../../../../../riemann-xi-function.md)

$$
\xi(s)=\tfrac12s(s-1)\Lambda(s)
$$

is [entire](../../../../../entire-function.md) and satisfies $\xi(s)=\xi(1-s)$. The reflection and duplication formulas for the [Gamma function](../../../../../gamma-function.md) turn the same identity into

$$
\boxed{\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s),}
$$

understood by [meromorphic continuation](../../../../../meromorphic-continuation.md) at removable exceptional points. This establishes the [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md), rather than assuming it.

If $N(T)$ counts zeros $\rho=\beta+i\gamma$ in the [critical strip](../../../../../critical-strip.md) with $0<\gamma\le T$, **including [zero multiplicity](../../../../../multiplicity-of-a-zero.md)**, the [Riemann–von Mangoldt formula](../../../../../riemann-von-mangoldt-formula.md) is

$$
\boxed{N(T)=\frac{T}{2\pi}\log\frac{T}{2\pi}-\frac{T}{2\pi}+O(\log T).}
$$

At a zero ordinate one may instead use the conventional half-weight boundary count; that only alters the stated error. In particular $N(T)\sim T\log T/(2\pi)$.

To invert without assuming simple zeros, fix $0<\varepsilon<1$ and set $T_n^\pm=(1\pm\varepsilon)2\pi n/\log n$. Then $\log T_n^\pm/\log n\to1$, so

$$
\frac{N(T_n^\pm)}n\longrightarrow1\pm\varepsilon.
$$

For large $n$, $N(T_n^-)<n<N(T_n^+)$, and hence $T_n^-<\gamma_n\le T_n^+$. Let $\varepsilon\downarrow0$. The [asymptotic inversion of the zeta zero count](../../../../../asymptotic-inversion-of-the-zeta-zero-count.md) gives

$$
\boxed{\gamma_n\sim\frac{2\pi n}{\log n}.}
$$

As in the zero-counting formula, the sequence lists ordinates with [zero multiplicity](../../../../../multiplicity-of-a-zero.md); “increasing” means nondecreasing here. The argument does not require the [Riemann hypothesis](../../../../../riemann-hypothesis.md) or simplicity of zeros.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
