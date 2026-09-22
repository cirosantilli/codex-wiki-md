<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

The [Wilson theorem](../../../../../wilson-s-theorem.md) states that for a prime $p$,

$$
(p-1)!\equiv-1\pmod p.
$$

Indeed, every nonzero residue modulo $p$ has a unique multiplicative inverse. The only residues equal to their own inverses solve $x^2\equiv1\pmod p$, hence are $1$ and $-1$. Pairing every other residue with its distinct inverse leaves

$$
(p-1)!\equiv1\cdot(-1)\equiv-1\pmod p.
$$

The [Fermat little theorem](../../../../../fermat-little-theorem.md) states that for prime $p$,

$$
a^p\equiv a\pmod p;
$$

equivalently, if $p\nmid a$, then $a^{p-1}\equiv1\pmod p$.

Wilson's theorem at $p=31$ gives

$$
30!=30\cdot29\cdot28!\equiv2\cdot28!\equiv-1\pmod{31},
$$

so $28!\equiv15\pmod{31}$. Also $729\equiv16\pmod{31}$, and therefore

$$
\boxed{28!\cdot729\equiv15\cdot16\equiv23\pmod{31}}.
$$

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
