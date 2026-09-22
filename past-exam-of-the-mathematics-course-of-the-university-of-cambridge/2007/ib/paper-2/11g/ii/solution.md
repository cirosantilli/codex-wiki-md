<h1 id="11g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**Hilbert's basis theorem:** if $R$ is a commutative [Noetherian ring](../../../../../../noetherian-ring.md) with identity, then the [polynomial ring](../../../../../../polynomial-ring.md) $R[x]$ is Noetherian. Iteration gives the same assertion for every finite number of variables.

Here is a [bounded-degree coefficient proof of Hilbert basis theorem](../../../../../../bounded-degree-coefficient-proof-of-hilbert-basis-theorem.md). Let $I$ be any [ideal](../../../../../../ideal.md) of $R[x]$. For $n\ge0$, define $J_n\subseteq R$ to be the coefficients of $x^n$ in the [polynomials](../../../../../../polynomial-split.md) of $I$ of degree at most $n$, including the zero coefficient. Closure under addition and scalar multiplication makes $J_n$ an [ideal](../../../../../../ideal.md) of $R$. Multiplication of a [polynomial](../../../../../../polynomial-split.md) by $x$ shows $J_n\subseteq J_{n+1}$. By the [ascending chain condition](../../../../../../ascending-chain-condition.md), there is $N$ such that $J_N=J_{N+1}=\cdots$.

Each $J_n$ for $0\le n\le N$ is finitely generated. Choose generators $a_{n,1},\ldots,a_{n,r_n}$ and corresponding [polynomials](../../../../../../polynomial-split.md) $f_{n,j}\in I$ of degree at most $n$ whose coefficient of $x^n$ is $a_{n,j}$. There are only finitely many chosen [polynomials](../../../../../../polynomial-split.md). We prove they generate $I$ by induction on degree.

Take a nonzero $f\in I$ of degree $d$ and leading coefficient $a$. If $d\le N$, express $a=\sum_jc_ja_{d,j}$ and subtract $\sum_jc_jf_{d,j}$. If $d>N$, use $a\in J_d=J_N$, express $a=\sum_jc_ja_{N,j}$, and subtract $\sum_jc_jx^{d-N}f_{N,j}$. In both cases the leading coefficient cancels, leaving a [polynomial](../../../../../../polynomial-split.md) in $I$ of smaller degree. For degree zero the remainder is zero, and the induction completes the claim.

Thus every [ideal](../../../../../../ideal.md) of $R[x]$ is finitely generated, proving the [Hilbert basis theorem](../../../../../../hilbert-basis-theorem.md). The proof uses no cancellation of nonzero elements of $R$, so it remains valid when $R$ has [zero divisors](../../../../../../zero-divisor.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11G](../../11g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
