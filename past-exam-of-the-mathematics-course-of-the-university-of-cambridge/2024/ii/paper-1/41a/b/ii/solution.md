<h1 id="41a/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Expanding the numerical propagation [matrix](../../../../../../../matrix.md),

$$
(I-kB)^{-1}(I-kC)^{-1}
=I+k(B+C)+k^2(B^2+BC+C^2)+O(k^3).
$$

Its difference from $e^{kA}$ is

$$
\frac{k^2}{2}(B^2+C^2+BC-CB)+O(k^3).
$$

Therefore the one-step local truncation error is

$$
\boxed{O(k^2),}
$$

and the method is first-order accurate globally.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
