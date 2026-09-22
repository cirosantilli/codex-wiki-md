# Elementary lower bound for the twin-prime sieve denominator

↑ **Parent:** [Polynomial root density in a sieve](polynomial-root-density-in-a-sieve.md)

For the [polynomial](polynomial-split.md) $F(n)=n(n+2)$, take $\rho(2)=1$ and $\rho(p)=2$ at odd [primes](prime-number.md). On odd [squarefree integers](squarefree-integer.md), the summand is at least $2^{\omega(d)}/d$. Put $y=\sqrt z$ and $L(y)=\sum_{a\le y,\ a\text{ odd}}1/a=\tfrac12\log y+O(1)$. The weight of odd pairs $a,b\le y$ is $L(y)^2$. The pairs for which $a$ is not [squarefree](squarefree-integer.md), $b$ is not [squarefree](squarefree-integer.md), or $(a,b)>1$ each have weight at most $L(y)^2\sum_{p\text{ odd}}p^{-2}$. Indeed, the weighted count of multiples of an odd $p^k$ is $p^{-k}L(y/p^k)\le p^{-k}L(y)$. Moreover,

$$
\sum_{p\text{ odd}}p^{-2}\le\sum_{m\ge1}(2m+1)^{-2}\le\frac19+\int_1^\infty\frac{dt}{(2t+1)^2}=\frac5{18}.
$$

Hence the odd [coprime](coprime-integers.md) [squarefree](squarefree-integer.md) pairs have weight at least $L(y)^2/6$. Their products $d=ab\le z$ are [squarefree](squarefree-integer.md), and $2^{\omega(d)}$ counts all ordered [coprime](coprime-integers.md) factorizations of $d$. This proves the displayed lower bound needed for the [Selberg upper-bound sieve](selberg-upper-bound-sieve.md).

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

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/4/solution.md)
