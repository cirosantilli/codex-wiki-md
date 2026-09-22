<h1 id="1e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [modular inverse](../../../../../../modular-multiplicative-inverse.md) of $2$ modulo $3$ is $2$, so the second [modular congruence](../../../../../../modular-congruence.md) is $x\equiv2\pmod3$. The third means $10\mid2(x-2)$, equivalently $5\mid x-2$. Cancelling this common factor changes the modulus; it gives $x\equiv2\pmod5$.

The first three conditions consequently combine to $x\equiv2\pmod{15}$ and $x$ odd, hence $x=17+30k$ for an [integer](../../../../../../integer.md) $k$. The last condition becomes

$$
30k\equiv10-17=-7\pmod{67}.
$$

As $30\cdot38=17\cdot67+1$, multiplying by the [modular inverse](../../../../../../modular-multiplicative-inverse.md) $38$ gives $k\equiv2\pmod{67}$. Thus

$$
\boxed{x=77+2010\ell,\qquad\ell\in\mathbb Z.}
$$

The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) states that [modular congruences](../../../../../../modular-congruence.md) with pairwise coprime moduli have a unique solution modulo their product. Here those moduli are $2,3,5,67$, with product $2010$. The derivation proves necessity, and substitution gives $77\equiv1\pmod2$, $2\cdot77\equiv1\pmod3$, $2\cdot77\equiv4\pmod{10}$ and $77\equiv10\pmod{67}$, proving sufficiency for the whole displayed class.

## ↑ Ancestors (11)

1. [B](../b.md)
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
