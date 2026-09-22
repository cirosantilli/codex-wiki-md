<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

Define the [Möbius function](../../../../../mobius-function.md) by $\mu(1)=1$, $\mu(n)=(-1)^r$ for a product of $r$ distinct primes, and $\mu(n)=0$ if a prime square divides $n$. For $n>1$, summing over square-free divisors gives $\sum_{d\mid n}\mu(d)=(1-1)^r=0$, while the sum is one at $n=1$.

Both [Dirichlet series](../../../../../dirichlet-series.md) $\sum n^{-s}$ and $\sum\mu(n)n^{-s}$ converge absolutely for $\sigma=\operatorname{Re}s>1$. Their product may therefore be regrouped by the product of the indices:

$$
\zeta(s)\sum_{n=1}^\infty\frac{\mu(n)}{n^s}
=\sum_{n=1}^\infty\frac{\sum_{d\mid n}\mu(d)}{n^s}=1.
$$

This simultaneously proves $\boxed{\zeta(s)\ne0\text{ for }\sigma>1}$ and

$$
\boxed{\frac1{\zeta(s)}=\sum_{n=1}^\infty\frac{\mu(n)}{n^s}.}
$$

In particular $|1/\zeta(\sigma+it)|\le\sum|\mu(n)|n^{-\sigma}\le\zeta(\sigma)$.

Under the assumed analytic continuation, $\zeta$ is holomorphic near $s_0=1+it_0$ when $t_0\ne0$, and $\zeta(\sigma)=1/(\sigma-1)+O(1)$ as $\sigma\downarrow1$. If $s_0$ were a zero of order $m\ge2$, local factorization would give $|1/\zeta(s_0+h)|\ge c h^{-m}$ for sufficiently small positive $h$. The preceding absolutely convergent bound gives instead $|1/\zeta(1+h+it_0)|=O(h^{-1})$, a contradiction. Thus $\boxed{m\le1}$. This [reciprocal Dirichlet-series bound on boundary-zero multiplicity](../../../../../reciprocal-dirichlet-series-bound-on-boundary-zero-multiplicity.md) does not assert that any such boundary zero exists.

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
