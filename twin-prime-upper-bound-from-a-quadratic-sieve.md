# Twin-prime upper bound from a quadratic sieve

↑ **Parent:** [Polynomial root density in a sieve](polynomial-root-density-in-a-sieve.md)

For $F(n)=n(n+2)$, every odd [prime](prime-number.md) has two forbidden [residue classes](residue-class.md). Use [Selberg sieve weights](selberg-sieve-weights.md) supported on odd [squarefree integers](squarefree-integer.md) $d\le R=x^{1/8}$. Their main quadratic form is $1/J$, where $J=\sum_{d\le R}\prod_{p\mid d}2/(p-2)$. The [truncated Euler-product lower bound](truncated-euler-product-lower-bound.md) applied to primes up to $R^{1/8}$ gives $J\gg\log^2R$: the mean logarithmic divisor size is $2\sum_{3\le p\le R^{1/8}}(\log p)/p<\frac12\log R$, by the [Mertens first theorem](mertens-first-theorem.md), and the full product is $\asymp\log^2R$, by the [Mertens second theorem](mertens-second-theorem.md). The [optimal Selberg weights have modulus at most one](optimal-selberg-weights-have-modulus-at-most-one.md), so the remainder is at most $O(\sum_{d,e\le R}[d,e])=O(R^4)$. The finitely many possible pairs with $p\le R$ contribute $O(R)$. Thus the count is $O(x/J+R^4+R)$, proving the bound.

## ↑ Ancestors (10)

1. [Polynomial root density in a sieve](polynomial-root-density-in-a-sieve.md)
2. [Selberg upper-bound sieve](selberg-upper-bound-sieve.md)
3. [Selberg sieve](selberg-sieve.md)
4. [Upper-bound sieve](upper-bound-sieve.md)
5. [Sieve theory](sieve-theory.md)
6. [Analytic number theory](analytic-number-theory-split.md)
7. [Number theory](number-theory-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Brun's theorem](brun-s-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-28/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/3/solution.md)
