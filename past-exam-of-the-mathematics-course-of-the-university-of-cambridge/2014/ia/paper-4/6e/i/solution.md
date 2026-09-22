<h1 id="6e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Fermat-Euler theorem](../../../../../../euler-s-theorem.md) states that, for an [integer](../../../../../../integer.md) $N\geq2$ and any [integer](../../../../../../integer.md) $a$ [coprime](../../../../../../coprime-integers.md) to $N$,

$$
\boxed{a^{\varphi(N)}\equiv1\pmod N,}
$$

where the [Euler totient function](../../../../../../euler-totient-function.md) $\varphi(N)$ counts the [residue classes](../../../../../../residue-class.md) [coprime](../../../../../../coprime-integers.md) to $N$.

Let $r_1,\ldots,r_{\varphi(N)}$ be representatives of these [residue classes](../../../../../../residue-class.md). Multiplication by $a$ gives a [permutation](../../../../../../permutation.md) of them: each $ar_i$ remains [coprime](../../../../../../coprime-integers.md) to $N$, and $ar_i\equiv ar_j$ implies $r_i\equiv r_j$ by cancellation using the [modular inverse](../../../../../../modular-multiplicative-inverse.md) of $a$. Multiplying all the resulting [modular congruences](../../../../../../modular-congruence.md) yields

$$
a^{\varphi(N)}r_1\cdots r_{\varphi(N)}\equiv r_1\cdots r_{\varphi(N)}\pmod N.
$$

The product is itself [coprime](../../../../../../coprime-integers.md) to $N$, so it has a [modular inverse](../../../../../../modular-multiplicative-inverse.md) and can be canceled. This proves the [Fermat-Euler theorem](../../../../../../euler-s-theorem.md). For $N=1$, the congruence is trivial; no separate argument is needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
