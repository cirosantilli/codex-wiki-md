<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Reduce the [polynomial](../../../../../polynomial-split.md) modulo $p$, obtaining a nonzero degree-$d$ [polynomial](../../../../../polynomial-split.md) over the field $\mathbb F_p$. If $a$ is a root, [polynomial](../../../../../polynomial-split.md) division gives $\bar f(X)=(X-a)h(X)$. Any different root $b$ is a root of $h$, because $b-a\ne0$ is invertible. Induction on degree therefore proves **there are at most $d$ distinct roots modulo $p$**.

Every nonzero residue is a root of $X^{p-1}-1$ by [Fermat's little theorem](../../../../../fermat-little-theorem.md). The difference between this monic [polynomial](../../../../../polynomial-split.md) and the product over all its $p-1$ nonzero roots has degree at most $p-2$, yet has $p-1$ roots. The root bound forces it to vanish identically over $\mathbb F_p$. Thus all coefficients of the corresponding integer [polynomial](../../../../../polynomial-split.md) are divisible by $p$.

For the requested failure modulo $p^2$, take $p=7$: $6!+1=721=7\cdot103$, and $103$ is not divisible by seven. Hence **the prime-square strengthening fails**, even though some special primes do satisfy it.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
