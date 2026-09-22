# Coefficient ideals of a polynomial ideal

↑ **Parent:** [Polynomial ring](polynomial-ring.md)

For an [ideal](ideal.md) $K\subseteq R[t]$, let $A_n(K)$ consist of the coefficients at $t^n$ of elements of $K$ of [polynomial degree](degree-of-a-polynomial.md) at most $n$, including the zero [polynomial](polynomial-split.md). Each $A_n(K)$ is an [ideal](ideal.md) of $R$, and multiplication of representing [polynomials](polynomial-split.md) by $t$ shows that $A_n(K)\subseteq A_{n+1}(K)$.

If $R$ is a [Noetherian ring](noetherian-ring.md), this chain stabilizes at some $N$. Choose finite [generating sets of an ideal](generating-set-of-an-ideal.md) for $A_0(K),\ldots,A_N(K)$, and for each nonzero generator choose a representing [polynomial](polynomial-split.md) $f_{nj}\in K$ with that [leading coefficient](leading-coefficient-of-a-polynomial.md) and [polynomial degree](degree-of-a-polynomial.md) $n$. These finitely many [polynomials](polynomial-split.md) generate $K$: for any nonzero $f\in K$ of [polynomial degree](degree-of-a-polynomial.md) $d$, use the chosen generators at level $\min(d,N)$, multiplied by suitable powers of $t$, to cancel its [leading coefficient](leading-coefficient-of-a-polynomial.md). Induction on [polynomial degree](degree-of-a-polynomial.md) finishes the argument. This proves the [Hilbert basis theorem](hilbert-basis-theorem.md) without assuming that $R$ is an [integral domain](integral-domain.md).

## ↑ Ancestors (6)

1. [Polynomial ring](polynomial-ring.md)
2. [Commutative algebra](commutative-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-commutative-algebra-course-of-the-university-of-oxford/2017/1/a/solution.md)
