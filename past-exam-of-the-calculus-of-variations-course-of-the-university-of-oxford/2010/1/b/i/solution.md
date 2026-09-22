<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**Zero is a strict weak local minimizer, but is not a strong local minimizer.** Put $D=\int_0^1|u'|^2\,dx$. Since $u(0)=0$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $|u(x)|^2\leq xD$, and therefore

$$
\int_0^1x^{2010}u(x)^2\,dx\leq\frac{D}{2012}.
$$

For sufficiently small $\|u'\|_\infty$, $\sin(u'^2)\geq\tfrac12u'^2$ [pointwise](../../../../../pointwise-convergence.md). Hence

$$
I(u)\geq\left(\frac12-\frac1{2012}\right)D\geq0,
$$

with equality only when $u=0$. Thus zero is a strict [weak local minimizer of a variational integral](../../../../../weak-local-minimizer-of-a-variational-integral.md).

For the strong claim, define a [Lipschitz](../../../../../lipschitz-continuity.md) triangular wave

$$
u_N(x)=\sqrt\pi\,\operatorname{dist}(x,N^{-1}\mathbb Z).
$$

It has zero endpoint values, $\|u_N\|_\infty=\sqrt\pi/(2N)\to0$, and $u_N'=\pm\sqrt\pi$ almost everywhere. Thus $\sin(u_N'^2)=\sin\pi=0$, while $u_N$ is nonzero on a set of positive measure. Consequently

$$
\boxed{I(u_N)=-\int_0^1x^{2010}u_N^2\,dx<0=I(0).}
$$

These uniformly small competitors disprove the [strong local minimizer of a variational integral](../../../../../strong-local-minimizer-of-a-variational-integral.md) property.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the calculus of variations course of the University of Oxford](../../../../split.md)
6. [Calculus of variations course of the University of Oxford](../../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
