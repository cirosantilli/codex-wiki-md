<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First the [eigenvalues](../../../../../../eigenvalue.md) of [Hecke operators](../../../../../../hecke-operator.md) are real. Here is the needed [Petersson inner product](../../../../../../petersson-inner-product.md) argument: unfold the finite coset sum defining $T_n$ into its correspondence domain, then change variables by each matrix. The determinant-normalized slash action preserves $y^k\,dx\,dy/y^2$ in the paired integrand, and transfers a representative to its inverse. Multiplying that inverse by the positive scalar $n$ gives its adjugate without changing the slash action. Adjugation reverses the integer determinant-$n$ correspondence, so the resulting sum is again $T_n$. Consequently $\langle T_nf,g\rangle=\langle f,T_ng\rangle$. Taking $g=f$ proves reality of $\lambda(n)$, since $\langle f,f\rangle>0$.

Fix one prime $p$ and set $x=\lambda(p)/p^{(k-1)/2}$ and $b_e=\lambda(p^e)/p^{e(k-1)/2}$. The [Hecke multiplication relations](../../../../../../hecke-multiplication-relations.md) proved in (a) give $b_0=1$, $b_1=x$ and $b_{e+2}=xb_{e+1}-b_e$. The distinct-root assumption excludes $x=\pm2$.

If $|x|<2$, write $x=2\cos\theta$, $0<\theta<\pi$. Solving the [linear recurrence](../../../../../../linear-recurrence-relation.md) gives $b_e=\sin((e+1)\theta)/\sin\theta$. If $\theta/(2\pi)$ is rational, infinitely many $e$ satisfy $(e+1)\theta\equiv\theta\pmod{2\pi}$, hence $b_e=1$. If it is irrational, density of the corresponding [irrational rotation](../../../../../../irrational-rotation.md) gives infinitely many $e$ in the open arc where $\sin((e+1)\theta)>\sin\theta/2$.

If $|x|>2$, let $\beta,\beta^{-1}$ be the real roots of $X^2-xX+1$, choosing $|\beta|>1$. Then $b_e=(\beta^{e+1}-\beta^{-e-1})/(\beta-\beta^{-1})$. Its even-index terms are positive and tend to infinity, whether $\beta$ is positive or negative. Thus the [prime-power coefficients of a level-one eigenform are often large and positive](../../../../../../prime-power-coefficients-of-a-level-one-eigenform-are-often-large-and-positive.md), and in either case

$$
\boxed{\lambda(p^e)\ge\tfrac12p^{e(k-1)/2}\text{ for infinitely many }e.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
