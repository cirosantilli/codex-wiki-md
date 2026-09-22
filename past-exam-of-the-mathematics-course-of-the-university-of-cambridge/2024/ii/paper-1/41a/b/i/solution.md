<h1 id="41a/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [matrix](../../../../../../../matrix.md) exponential is the absolutely convergent [series](../../../../../../../series-mathematics.md)

$$
e^X=\sum_{j=0}^\infty\frac{X^j}{j!}.
$$

Multiplying the two expansions gives

$$
e^{kB}e^{kC}
=I+k(B+C)+k^2\left(\frac12B^2+BC+\frac12C^2\right)+O(k^3).
$$

On the other hand,

$$
e^{k(B+C)}
=I+k(B+C)+\frac{k^2}{2}(B^2+BC+CB+C^2)+O(k^3).
$$

Subtracting yields

$$
\boxed{
e^{kB}e^{kC}=e^{k(B+C)}
+\frac{k^2}{2}(BC-CB)+O(k^3).}
$$

This is the leading [Lie-Trotter splitting commutator error](../../../../../../../lie-trotter-splitting-commutator-error.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [41A](../../../41a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
