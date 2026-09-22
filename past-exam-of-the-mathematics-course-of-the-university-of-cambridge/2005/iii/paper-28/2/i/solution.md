<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With the normalization of the preceding completion, the super-completion is the [Riemann xi function](../../../../../../riemann-xi-function.md)

$$
\boxed{\xi(s)=\frac12s(s-1)\Xi(s)
=\frac12s(s-1)\pi^{-s/2}\Gamma(s/2)\zeta(s).}
$$

The [pole-subtracted theta integral for the completed zeta function](../../../../../../pole-subtracted-theta-integral-for-the-completed-zeta-function.md) gives the particularly useful expression

$$
\xi(s)=\frac12+\frac14s(s-1)\bigl(J(s)+J(1-s)\bigr).
$$

It proves directly that $\xi$ is an [entire function](../../../../../../entire-function.md), with $\xi(0)=\xi(1)=1/2$ and $\xi(s)=\xi(1-s)$. Here “integral function” means entire, not integer-valued.

To prove the [order-one growth of the Riemann xi function](../../../../../../order-one-growth-of-the-riemann-xi-function.md), put $M(R)=\max_{|s|\leq R}|\xi(s)|$. For $R\geq3$, the exponentially decreasing theta integrand bounds both $J(s)$ and $J(1-s)$ by

$$
C\int_1^\infty e^{-\pi u}u^{(R+1)/2-1}\,du
\leq C\pi^{-(R+1)/2}\Gamma((R+1)/2).
$$

Multiplication by the quadratic factor in $s$ and the [Stirling formula](../../../../../../stirling-formula.md) imply $\log M(R)=O(R\log R)$. Hence the [order of an entire function](../../../../../../order-of-an-entire-function.md) is at most one. On the positive real axis, $\zeta(R)=1+O(2^{-R})$, and the defining formula and [Stirling formula](../../../../../../stirling-formula.md) give

$$
\log\xi(R)=\frac R2\log R+O(R).
$$

This lower bound proves that the order is at least one. Consequently **$\xi$ is entire of order exactly one**, generally not of finite exponential type.

Its zeros are precisely the [Nontrivial zeros of the Riemann zeta function](../../../../../../nontrivial-zero-of-the-riemann-zeta-function.md), counted with multiplicity. The values at zero and one are nonzero; the [Gamma function](../../../../../../gamma-function.md) has no zeros; and the completed [functional equation](../../../../../../functional-equation.md) together with the [Euler product](../../../../../../euler-product.md) shows that there are no further completed zeros outside the closed critical strip. By [Hadamard factorization](../../../../../../hadamard-factorization-theorem.md) for entire functions of order one,

$$
\xi(s)=e^{A+Bs}\prod_\rho\left(1-\frac{s}{\rho}\right)e^{s/\rho},
\qquad e^A=\frac12,\quad B=\frac{\xi'(0)}{\xi(0)}.
$$

The genus-one factors give $\sum_\rho|\rho|^{-2}<\infty$, and the [logarithmic derivative](../../../../../../logarithmic-derivative.md) converges locally normally away from the zeros:

$$
\frac{\xi'(s)}{\xi(s)}
=B+\sum_\rho\left(\frac1{s-\rho}+\frac1\rho\right).
$$

Differentiate the defining product of $s(s-1)$, the gamma factor, and $\zeta(s)$. Rearranging proves the [global partial-fraction expansion of the zeta logarithmic derivative](../../../../../../global-partial-fraction-expansion-of-the-zeta-logarithmic-derivative.md):

$$
\boxed{\frac{\zeta'(s)}{\zeta(s)}
=B-\frac1s-\frac1{s-1}+\frac12\log\pi
-\frac12\frac{\Gamma'(s/2)}{\Gamma(s/2)}
+\sum_\rho\left(\frac1{s-\rho}+\frac1\rho\right).}
$$

The summands must be kept together: each is $O_s(|\rho|^{-2})$ for large $|\rho|$, whereas separating the two complex reciprocal sums need not preserve [absolute convergence](../../../../../../absolute-convergence.md). The gamma term accounts for the trivial zeros as well as cancellation at zero.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
