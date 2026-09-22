<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Build the spherical system by adding shells from the centre outwards. The [shell theorem](../../../../../../spherical-shell-theorem.md) says that a shell of mass $dM$ at radius $r$ interacts with the already assembled interior mass through potential $-GM(r)/r$. Thus its contribution is $dW=-GM(r)dM(r)/r$. Each pair is counted when its outer member is added, so no further factor of one half is needed:

$$
W=-G\int_0^\infty\frac{M(r)}r\,dM(r)
=-\frac G2\int_0^\infty\frac1r\,d[M(r)^2].
$$

Integration by parts gives

$$
W=-\frac G2\left[\frac{M(r)^2}r\right]_0^\infty
-\frac G2\int_0^\infty\frac{M(r)^2}{r^2}\,dr.
$$

For an isolated finite-mass system without a singular central point mass, the endpoint term vanishes provided the central cusp has finite binding energy. Consequently

$$
\boxed{W=-\frac G2\int_0^\infty\frac{M(r)^2}{r^2}\,dr.}
$$

This is the [spherical binding-energy mass integral](../../../../../../spherical-binding-energy-mass-integral.md). If a central singularity makes the endpoint or integral divergent, the finite-energy assumption must be checked rather than silently discarding that term.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
