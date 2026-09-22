<h1 id="13d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $z=R+iy$, $0\leq y\leq\pi$, the numerator modulus is $e^{-2Ry/\pi}$ and the denominator modulus is at least $1-e^{-2R}$. Hence the magnitude of the right-side [contour integral](../../../../../../contour-integral.md) is at most

$$
\frac1{1-e^{-2R}}\int_0^\pi e^{-2Ry/\pi}\,dy=\frac\pi{2R}.
$$

On $z=-R+iy$ the corresponding bounds are $e^{2Ry/\pi}$ and $e^{2R}-1$, giving exactly the same bound $\pi/(2R)$. Thus **the total vertical contribution is $O(R^{-1})$ and vanishes**. This integral estimate handles the endpoints where a pointwise uniform-decay argument would fail.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [13D](../../13d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
