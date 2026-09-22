<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $F(m)=m(m+2)(m+6)$ and let $\rho(d)$ be the number of roots of $F$ modulo $d$. For squarefree $d$, the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) gives

$$
\rho(d)=\prod_{p\mid d}\rho(p),
\qquad
\rho(2)=1,quad \rho(3)=2,quad \rho(p)=3\quad(p\geq5).
$$

Indeed, for $p\geq5$ the three roots $0,-2,-6$ are distinct. Counting $m\leq X$ in each of the $\rho(d)$ residue classes gives

$$
|\mathcal A_d|
=\#\{m\leq X:d\mid F(m)\}
=\frac{\rho(d)}dX+O(\rho(d)).
$$

Consequently a suitable [sieve distribution](../../../../../../sieve-distribution.md) is

$$
g(d)=\frac{\rho(d)}d,
\qquad
r_d=O(\rho(d))=O(3^{\omega(d)}).
$$

This is the [polynomial root density in a sieve](../../../../../../polynomial-root-density-in-a-sieve.md) calculation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
