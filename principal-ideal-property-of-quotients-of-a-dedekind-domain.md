# Principal ideal property of quotients of a Dedekind domain

↑ **Parent:** [Dedekind domain](dedekind-domain.md)

For a [Dedekind domain](dedekind-domain.md) $R$ and a nonzero proper [ideal](ideal.md) $I$, the [quotient ring](quotient-ring.md) $R/I$ is a [principal ideal ring](principal-ideal-ring.md). First, the [correspondence theorem for ideals](correspondence-theorem-for-ideals.md) and [unique factorization of ideals in a Dedekind domain](unique-factorization-of-ideals-in-a-dedekind-domain.md) show that the [ideals](ideal.md) of $R/P^n$ are exactly $P^i/P^n$, $0\leq i\leq n$. Consecutive powers are distinct by cancellation of [invertible fractional ideals](invertible-fractional-ideal.md). Choose $\pi\in P^i\setminus P^{i+1}$. There is no intermediate [ideal](ideal.md) between these consecutive powers, so $P^i=(\pi)+P^{i+1}$. Multiplication by $P^r$ and substitution show inductively that $P^i=(\pi)+P^{i+r}$ for every $r\geq1$. Taking $r=n-i$ gives a single generator modulo $P^n$. Now factor $I$ into pairwise [comaximal ideals](comaximal-ideals.md) $P_j^{n_j}$. The [Chinese remainder theorem](chinese-remainder-theorem.md) writes $R/I$ as a finite [direct product of rings](direct-product-of-rings.md) of the preceding type, which is a [principal ideal ring](principal-ideal-ring.md). It need not be an [integral domain](integral-domain.md), as $\mathbb Z/4\mathbb Z$ demonstrates. Applying the result to $(a)$ for any $0\ne a\in I$ makes $I/(a)$ cyclic, yielding [two generators for an ideal in a Dedekind domain](two-generators-for-an-ideal-in-a-dedekind-domain.md).

## ↑ Ancestors (6)

1. [Dedekind domain](dedekind-domain.md)
2. [Commutative algebra](commutative-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebraic-number-theory-course-of-the-university-of-oxford/2023/2/b/iii/solution.md)
