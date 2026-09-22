<h1 id="7e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $d$ be the [multiplicative order](../../../../../../multiplicative-order.md) of $a$ modulo $p$. Use [Euclidean division](../../../../../../euclidean-division.md) to write $x=qd+r$, $0\le r<d$. Since $a^d\equiv1$,

$$
a^x\equiv a^r\pmod p.
$$

If $a^x\equiv1$, minimality of $d$ forces $r=0$, so **$d$ divides $x$**. Conversely, $d\mid x$ immediately gives $a^x\equiv1$. For negative [integers](../../../../../../integer.md) $x$, powers are interpreted using the [multiplicative inverse](../../../../../../multiplicative-inverse.md) and the same argument applies.

Apply the result to $x=p-1$, using [Fermat's little theorem](../../../../../../fermat-little-theorem.md). Then $d\mid p-1$, equivalently

$$
\boxed{p\equiv1\pmod d.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7E](../../7e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
