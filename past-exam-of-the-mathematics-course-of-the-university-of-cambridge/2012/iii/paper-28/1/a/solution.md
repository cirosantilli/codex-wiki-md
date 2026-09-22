<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Every [Non-Archimedean absolute value](../../../../../../non-archimedean-absolute-value.md) on $\mathbb Q$ is either the [trivial absolute value](../../../../../../trivial-absolute-value.md), or $|\cdot|_p^c$ for a unique prime $p$ and some $c>0$. Here $|p|_p=p^{-1}$.

To prove this classification, the ultrametric inequality gives $|n|\leq1$ for all integers $n$. If every nonzero integer has absolute value one, multiplicativity makes the [absolute value on a field](../../../../../../absolute-value-algebra.md) trivial on all rational numbers. Otherwise some positive integer has absolute value less than one, and its prime factorization gives a prime $p$ with $0<|p|<1$. There cannot be two such primes: if $p\ne q$ and $ap+bq=1$ with integers $a,b$, then $1\leq\max(|p|,|q|)<1$, a contradiction. Every other prime consequently has absolute value one. Unique prime factorization now gives

$$
|x|=|p|^{v_p(x)}=p^{-c v_p(x)},\qquad c=-\frac{\log|p|}{\log p}>0.
$$

Conversely these are [Non-Archimedean absolute values](../../../../../../non-archimedean-absolute-value.md), by the valuation inequality $v_p(x+y)\geq\min(v_p(x),v_p(y))$. **Thus $\boxed{|\cdot|=|\cdot|_p^c\ (c>0)\text{ or the trivial value}}$.** This is the non-Archimedean part of [Ostrowski theorem](../../../../../../ostrowski-s-theorem.md), including the trivial case.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
