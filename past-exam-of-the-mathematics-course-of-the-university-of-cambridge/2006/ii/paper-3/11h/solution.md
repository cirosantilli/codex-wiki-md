<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

The [Prime number theorem](../../../../../prime-number-theorem.md) states that $\pi(x)\sim x/\log x$, where $\pi(x)$ counts [primes](../../../../../prime-number.md) not exceeding $x$. [Dirichlet theorem on primes in arithmetic progressions](../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md) states that if $\gcd(a,m)=1$, then the progression $a+jm$ contains infinitely many [primes](../../../../../prime-number.md).

If $x^2\equiv-1\pmod p$ for an odd [prime](../../../../../prime-number.md) $p$, the multiplicative order of $x$ modulo $p$ is four. [Lagrange's theorem](../../../../../lagrange-s-theorem.md) therefore gives $4\mid p-1$. Conversely, [Wilson's theorem](../../../../../wilson-s-theorem.md) gives $(p-1)!\equiv-1\pmod p$. Pairing the factors $j$ and $p-j$ yields

$$
(-1)^{(p-1)/2}\left(\left(\frac{p-1}{2}\right)!\right)^2\equiv-1\pmod p.
$$

For $p\equiv1\pmod4$, the sign is positive, so the factorial supplies a square root of $-1$. Thus **$-1$ is a quadratic residue exactly when $p\equiv1\pmod4$**.

Write $P=\prod_jp_j$. The odd integer $4P-1$ is $3$ modulo $4$. If all of its [prime factors](../../../../../prime-factor.md) were $1$ modulo $4$, their product, with multiplicities, would be $1$ modulo $4$, so at least one factor is $3$ modulo $4$. Every [prime factor](../../../../../prime-factor.md) $q$ of $4P^2+1$ is odd and satisfies $(2P)^2\equiv-1\pmod q$; the criterion just proved gives $q\equiv1\pmod4$. Neither integer is divisible by any $p_j$, since their residues modulo $p_j$ are respectively $-1$ and $1$. Starting with any finite list thus produces a new [prime](../../../../../prime-number.md) in each residue class. **Both classes contain infinitely many primes**, independently of the general [Dirichlet theorem on primes in arithmetic progressions](../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md).

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
