<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For coefficients $b_n$ supported on an interval of length $H$, write $B=\sum b_n$ and $B_p(a)=\sum_{n\equiv a\pmod p}b_n$. The [variance form of the large sieve](../../../../../../variance-form-of-the-large-sieve.md) states

$$
\sum_{p\leq Q}p\sum_{a\bmod p}|B_p(a)-B/p|^2\ll(H+Q^2)\sum|b_n|^2.
$$

The constant is absolute. One may take the explicit right side $(Q^2+2\pi H)\sum|b_n|^2$, by [orthogonality of roots of unity](../../../../../../orthogonality-of-roots-of-unity.md) and the [exponential-sum large sieve](../../../../../../exponential-sum-large-sieve.md) proved in Question 2.

Take $H=\lfloor N^2\rfloor$, $Q=N$, and $b_n$ the [indicator function](../../../../../../indicator-function.md) of the $N^\varepsilon$-[smooth numbers](../../../../../../smooth-number.md) up to $N^2$. Applying the given smooth-number density with parameter $\varepsilon/2$ gives

$$
B\geq\kappa(\varepsilon/2)N^2,
$$

with a harmless adjustment of the constant for integer endpoints. If an [odd prime](../../../../../../odd-prime.md) $p\leq N$ has [least quadratic nonresidue](../../../../../../least-quadratic-nonresidue.md) $n(p)>N^\varepsilon$, then $p>N^\varepsilon$: a [quadratic nonresidue](../../../../../../quadratic-nonresidue.md) always occurs among $1,\ldots,p-1$. Every [prime factor](../../../../../../prime-factor.md) of every selected [smooth number](../../../../../../smooth-number.md) is thus a nonzero [quadratic residue](../../../../../../quadratic-residue.md) modulo $p$. By the [multiplicativity of the Legendre symbol](../../../../../../multiplicativity-of-the-legendre-symbol.md), every selected number is a nonzero [quadratic residue](../../../../../../quadratic-residue.md) modulo $p$.

There are $(p-1)/2$ nonzero [quadratic nonresidue](../../../../../../quadratic-nonresidue.md) classes, and $B_p(a)=0$ on all of them. Their contribution to the variance is at least

$$
p\frac{p-1}{2}\left(\frac Bp\right)^2
=\frac{p-1}{2p}B^2\geq\frac13B^2.
$$

If $R$ denotes the number of exceptional [primes](../../../../../../prime-number.md), the [variance form of the large sieve](../../../../../../variance-form-of-the-large-sieve.md), with $\sum|b_n|^2=B$, yields $RB^2\ll N^2B$. Consequently

$$
\boxed{R\ll\frac{N^2}{B}\ll\kappa(\varepsilon/2)^{-1}=O_\varepsilon(1).}
$$

This is the [bounded exceptional primes for least quadratic nonresidues](../../../../../../bounded-exceptional-primes-for-least-quadratic-nonresidues.md) argument. Using an interval of length $N^2$ is what matches the $Q^2$ term; an interval of length $N$ would not give a bounded exceptional set.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
