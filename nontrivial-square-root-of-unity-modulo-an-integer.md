# Nontrivial square root of unity modulo an integer

↑ **Parent:** [Congruence of squares](congruence-of-squares.md)

For an odd [integer](integer-split.md) $N>1$, a nontrivial square root of unity modulo $N$ is a residue $z$ with $z^2\equiv1\pmod N$ and $z\not\equiv\pm1\pmod N$. Then both $\gcd(z-1,N)$ and $\gcd(z+1,N)$ are proper [divisors](divisor.md). For $N=77$, $z=34$ works: $34^2\equiv1\pmod{77}$, $\gcd(33,77)=11$, and $\gcd(35,77)=7$.

A [congruence of squares](congruence-of-squares.md) with $\gcd(b,N)=1$ converts to this form by $z\equiv a b^{-1}\pmod N$, using a [modular multiplicative inverse](modular-multiplicative-inverse.md). In the $a=20,b=13$ example, $13^{-1}\equiv6\pmod{77}$, so $z\equiv20\cdot6\equiv43\pmod{77}$. It yields $\gcd(42,77)=7$ and $\gcd(44,77)=11$. Nontriviality requires mixed sign choices across prime factors, which an odd [prime number](prime-number-split.md) modulus cannot provide.

## ↑ Ancestors (6)

1. [Congruence of squares](congruence-of-squares.md)
2. [Integer factorization](integer-factorization.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
