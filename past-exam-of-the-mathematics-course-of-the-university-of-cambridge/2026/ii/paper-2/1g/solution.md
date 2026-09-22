<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

The [möbius function](../../../../../mobius-function.md) is $mu(1)=1$, $mu(n)=0$ if a prime square divides $n$, and $mu(n)=(-1)^r$ when $n$ is a product of $r$ distinct primes. The [Riemann zeta function](../../../../../riemann-zeta-function.md) is $zeta(s)=\sum_{n\ge1}n^{-s}$ for $\Re s>1$.

Both sides of the proposed identity are multiplicative. At $n=p^a$, the right side is $1$ for $a=0,1$ and $1+\mu(p)=0$ for $a\ge2$, exactly $mu(p^a)^2$. Absolute convergence permits rearrangement, so

$$
\boxed{\sum_n\frac{\mu(n)^2}{n^s}=\sum_d\frac{\mu(d)}{d^{2s}}\sum_m\frac1{m^s}=\frac{\zeta(s)}{\zeta(2s)}.}
$$

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
