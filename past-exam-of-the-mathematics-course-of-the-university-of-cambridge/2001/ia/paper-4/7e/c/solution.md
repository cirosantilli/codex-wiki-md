<h1 id="7e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $x^2\equiv-1\pmod p$ with $p$ an [odd prime](../../../../../../odd-prime.md), then $x^4\equiv1$ but $x^2\not\equiv1$. The [multiplicative order](../../../../../../multiplicative-order.md) consequently divides four and is neither one nor two, so it is **four**. The preceding divisibility result makes $4\mid p-1$ necessary.

For sufficiency, suppose $p\equiv1\pmod4$ and put $r=(p-1)/2$, an [even integer](../../../../../../even-number.md). Pair opposite factors in the [factorial](../../../../../../factorial.md):

$$
(p-1)!=\prod_{j=1}^rj(p-j)\equiv(-1)^r(r!)^2=(r!)^2\pmod p.
$$

[Wilson's theorem](../../../../../../wilson-s-theorem.md) gives $(r!)^2\equiv-1\pmod p$, explicitly producing a [square root of minus one modulo a prime](../../../../../../square-root-of-minus-one-modulo-a-prime.md). Thus

$$
\boxed{\text{For odd }p,\quad x^2\equiv-1\pmod p\text{ is soluble }\Longleftrightarrow p\equiv1\pmod4.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
