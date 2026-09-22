<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[summation by parts](../../../../abel-s-summation-formula.md), with $S(x)=\sum_{n\leq x}\chi(n)$, gives for an [integer](../../../../integer-split.md) $N$

$$
\sum_{n\leq N}\chi(n)n^{-s}
=S(N)N^{-s}+s\int_1^N S(x)x^{-s-1}\,dx.
$$

The boundary term tends to zero when $\operatorname{Re}s>0$ because $S$ is bounded. In the original region of [absolute convergence](../../../../absolute-convergence.md) this proves

$$
\boxed{L(s)=s\int_1^\infty S(x)x^{-s-1}\,dx.}
$$

For a [compact subset](../../../../compact-space.md) of $\operatorname{Re}s>0$, choose $\delta>0$ below all its real parts and bound $|s|$ there. The integral tail is bounded by a constant times $\int_N^\infty x^{-1-\delta}dx$, uniformly on that [compact set](../../../../compact-space.md). Its truncated integrals are [holomorphic function](../../../../holomorphic-function-split.md) in $s$, so [locally uniform convergence](../../../../locally-uniform-convergence.md) proves a [analytic continuation](../../../../analytic-continuation.md) throughout $\operatorname{Re}s>0$. This is [holomorphy of a Dirichlet series from bounded partial sums](../../../../holomorphy-of-a-dirichlet-series-from-bounded-partial-sums.md).

The [Euler product](../../../../euler-product.md), valid for $\operatorname{Re}s>1$, is

$$
L(s)=\prod_p(1-\chi(p)p^{-s})^{-1}
=\prod_{p\equiv1\ (4)}(1-p^{-s})^{-1}
\prod_{p\equiv3\ (4)}(1+p^{-s})^{-1}.
$$

Expand the logarithms of these absolutely convergent [Euler products](../../../../euler-product.md). Writing $\theta=mt\log p$, the logarithm of the product in the desired inequality is

$$
\sum_p\sum_{m\geq1}\frac{
3+4\chi(p)^m\cos\theta+\cos2\theta}{m p^{m\sigma}}.
$$

For odd $p$, $\chi(p)^m$ is $1$ or $-1$. In the first case the numerator is the given nonnegative trigonometric [polynomial](../../../../polynomial-split.md). In the second replace $\theta$ by $\theta+\pi$, which changes the sign of $\cos\theta$ and leaves $\cos2\theta$ unchanged. At $p=2$ the numerator is $3+\cos2\theta\geq2$. Every summand is nonnegative. Exponentiation proves

$$
\boxed{\zeta(\sigma)^3|L(\sigma+it)|^4
|\zeta(\sigma+2it)|\geq1.}
$$

This is the [three-four-one inequality for Euler products](../../../../three-four-one-inequality-for-euler-products.md) applied to the real character modulo four.

Suppose $t\neq0$ and $L(1+it)=0$. Holomorphy gives $L(\sigma+it)=O(\sigma-1)$ as $\sigma\downarrow1$. The only pole of the [Riemann zeta function](../../../../riemann-zeta-function.md) is at one, so $\zeta(\sigma+2it)$ remains bounded, while $\zeta(\sigma)^3=O((\sigma-1)^{-3})$. The displayed product is then $O(\sigma-1)$, contradicting its lower bound. Hence **$L(1+it)\neq0$ for $t\neq0$**.

At $t=0$ the last zeta factor also has a pole, so that contradiction no longer follows from the inequality. Instead evaluate the convergent alternating series:

$$
L(1)=1-\frac13+\frac15-\cdots
=\int_0^1\frac{dx}{1+x^2}
=\boxed{\frac\pi4\neq0}.
$$

For rigor, integrate the finite geometric identity for $(1+x^2)^{-1}$; the remainder has absolute integral at most $1/(2N+3)$ and tends to zero. [summation by parts](../../../../abel-s-summation-formula.md) above identifies this value with the [analytic continuation](../../../../analytic-continuation.md) at one.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
