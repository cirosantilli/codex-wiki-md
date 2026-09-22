<h1 id="11g/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By [Euler criterion](../../../../../../../euler-criterion.md),

$$
T\equiv\sum_{a=1}^{p-1}a^{(p+1)/2}\pmod p.
$$

Choose a [primitive root](../../../../../../../primitive-root-modulo-n.md) $g$. For any integer $m$ not divisible by $p-1$,

$$
\sum_{a=1}^{p-1}a^m
=\sum_{j=0}^{p-2}g^{jm}
=\frac{g^{m(p-1)}-1}{g^m-1}
\equiv0\pmod p.
$$

For $p>3$, the exponent $m=(p+1)/2$ satisfies $0<m<p-1$. Therefore

$$
\boxed{T\equiv0\pmod p.}
$$

Together with part (i), this is the [weighted complete Legendre-symbol sum](../../../../../../../weighted-complete-legendre-symbol-sum.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [11G](../../../11g.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
