<h1 id="1e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since $31$ is a [prime number](../../../../../../prime-number.md), the [Wilson theorem](../../../../../../wilson-s-theorem.md) states that $30!\equiv-1\pmod{31}$. But $30!\equiv(-1)(-2)28!=2\cdot28!$, so the [modular inverse](../../../../../../modular-multiplicative-inverse.md) of $2$, which is $16$, gives

$$
28!\equiv-16\equiv15\pmod{31}.
$$

The [Fermat little theorem](../../../../../../fermat-little-theorem.md) states that $a^{p-1}\equiv1\pmod p$ when $p$ is prime and $p\nmid a$. Therefore $13^{30}\equiv1\pmod{31}$, and

$$
13^{28}\equiv(13^2)^{-1}\equiv14^{-1}\equiv20\pmod{31},
$$

since $14\cdot20=280=9\cdot31+1$. Combining these [modular congruences](../../../../../../modular-congruence.md),

$$
28!13^{28}\equiv15\cdot20=300\equiv\boxed{21}\pmod{31}.
$$

This representative lies between $0$ and $30$, so it is the least nonnegative residue.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1E](../../1e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
