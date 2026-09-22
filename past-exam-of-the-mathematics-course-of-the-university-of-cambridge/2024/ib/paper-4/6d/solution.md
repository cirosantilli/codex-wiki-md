<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

On each interval of width $h=1/N$, Taylor expansion about its midpoint shows that the local midpoint-rule error is $O(h^3)$. Summing over $N$ intervals gives the [composite midpoint rule error](../../../../../composite-midpoint-rule-error.md)

$$
\boxed{I(f)-I_N(f)=O(N^{-2})}.
$$

To remove the endpoint singularity, set $x=s^2$. Then

$$
I(f)=\int_0^1 2s f(s^2)\,ds
=\int_0^1 2g(s^2)\,ds,
$$

whose transformed integrand is analytic. Applying the composite midpoint rule in $s$ with $s_n=(n+\tfrac12)/N$ gives

$$
I(f)\approx\frac2N\sum_{n=0}^{N-1}s_nf(s_n^2).
$$

This has the required form when

$$
\boxed{y_n=s_n^2
=\left(\frac{n+\tfrac12}{N}\right)^2}.
$$

The [quadratic substitution for a square-root endpoint singularity](../../../../../quadratic-substitution-for-a-square-root-endpoint-singularity.md) therefore restores second-order convergence.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
