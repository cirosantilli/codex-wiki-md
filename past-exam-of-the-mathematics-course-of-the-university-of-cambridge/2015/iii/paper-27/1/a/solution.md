<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $L=\sqrt D$. Regroup the finite [divisor sum](../../../../../../divisor-sum.md) using the [least common multiple](../../../../../../least-common-multiple.md):

$$
\sum_{d\mid n}\lambda_d
=\sum_{[u,v]\mid n}\rho_u\rho_v
=\left(\sum_{d\mid n}\rho_d\right)^2.
$$

This is nonnegative. If $n$ has no [prime factor](../../../../../../prime-factor.md) in $\mathcal P$, only $d=1$ can contribute to the inner [sum](../../../../../../sum.md), so it equals $\rho_1=1$. This proves the required pointwise [upper-bound sieve](../../../../../../upper-bound-sieve.md) inequality. Whenever a term defining $\lambda_d$ is nonzero, $u,v\leq L$ and their [prime factors](../../../../../../prime-factor.md) lie in $\mathcal P$. Hence $d=[u,v]\leq uv\leq L^2=D$, and every [prime factor](../../../../../../prime-factor.md) of $d$ lies in $\mathcal P$. Thus these are **upper-bound sieve weights of level $D$**, as described by the [Selberg least-common-multiple weights](../../../../../../selberg-least-common-multiple-weights.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
