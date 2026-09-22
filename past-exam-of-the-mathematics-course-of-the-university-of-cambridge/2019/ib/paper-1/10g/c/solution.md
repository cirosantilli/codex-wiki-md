<h1 id="10g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interchange the two primes if necessary so that $p<q$. By the [Sylow theorems](../../../../../../sylow-theorems.md), the number $n_q$ of Sylow $q$-subgroups satisfies

$$
n_q\mid p^2,
\qquad
n_q\equiv1\pmod q.
$$

If $n_q\ne1$, then $n_q$ is $p$ or $p^2$. The first is impossible because $1<p<q$. The second would imply

$$
q\mid p^2-1=(p-1)(p+1).
$$

Since $q>p$ is prime, it cannot divide $p-1$, so it must divide $p+1$. But $q>p$ then forces $q=p+1$, impossible because $p$ and $q$ are both odd. Therefore $n_q=1$. The unique Sylow $q$-subgroup is a nontrivial proper [normal subgroup](../../../../../../normal-subgroup.md), and hence

$$
\boxed{G\text{ is not simple}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10G](../../10g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
