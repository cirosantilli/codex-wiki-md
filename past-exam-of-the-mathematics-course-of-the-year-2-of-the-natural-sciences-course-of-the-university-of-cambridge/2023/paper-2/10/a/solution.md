<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The upper-left block of $U$ is the planar [rotation matrix](../../../../../rotation-matrix.md) $R(\pi/2)$, and $U$ fixes the third coordinate. Therefore

$$
U^p=\begin{pmatrix}\cos(p\pi/2)&-\sin(p\pi/2)&0\\\sin(p\pi/2)&\cos(p\pi/2)&0\\0&0&1\end{pmatrix},\qquad U^4=I.
$$

The diagonal entries of $V$ square to one, so $V^2=I$. Direct conjugation gives $VUV=U^{-1}$, hence $VU^pV=U^{-p}$ for every integer $p$. Consequently

$$
\boxed{U^pV=VU^{-p}=VU^{4-(p\bmod4)}.}
$$

When $p\bmod4=0$, the last exponent is four, which is equivalent to zero because $U^4=I$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
