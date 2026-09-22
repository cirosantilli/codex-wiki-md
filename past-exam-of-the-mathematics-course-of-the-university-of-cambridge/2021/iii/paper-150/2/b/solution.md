<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The functional equation is

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s)}.
$$

Equivalently,

$$
\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s).
$$

For a proof, let

$$
\Theta(u)=\sum_{n\in\mathbb Z}e^{-\pi n^2u}.
$$

The [Poisson summation formula](../../../../../../poisson-summation-formula.md) applied to a [Gaussian function](../../../../../../gaussian-function.md) gives the theta transformation

$$
\Theta(u)=u^{-1/2}\Theta(1/u).
$$

The standard [Gamma function](../../../../../../gamma-function.md) integral and termwise integration initially give, for $\Re s>1$,

$$
\Lambda(s):=\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\frac12\int_0^\infty(\Theta(u)-1)u^{s/2}\frac{du}{u}.
$$

Split the integral at one, substitute $u\mapsto1/u$ in the lower half, and use the theta transformation. The result is

$$
\Lambda(s)=\frac1{s(s-1)}
+\frac12\int_1^\infty(\Theta(u)-1)
\left(u^{s/2}+u^{(1-s)/2}\right)\frac{du}{u}.
$$

The integral is an [entire function](../../../../../../entire-function.md) of $s$ because $\Theta(u)-1$ decays exponentially. The right side is visibly invariant under $s\mapsto1-s$, proving both the [analytic continuation](../../../../../../analytic-continuation.md) and the [functional equation of the Riemann zeta function](../../../../../../functional-equation-of-the-riemann-zeta-function.md). This is the [Mellin representation of the completed Riemann zeta function](../../../../../../mellin-representation-of-the-completed-riemann-zeta-function.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
