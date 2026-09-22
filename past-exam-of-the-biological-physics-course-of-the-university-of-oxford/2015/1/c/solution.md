<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Normalize both [fluorescent reporter](../../../../fluorescent-reporter.md) intensities by their respective means, correcting unequal brightness and background, and denote them $c,y$. [Extrinsic gene-expression noise](../../../../extrinsic-gene-expression-noise.md) changes shared cellular conditions and moves both signals together: the scatter is a long narrow cloud around $y=c$. [Intrinsic gene-expression noise](../../../../intrinsic-gene-expression-noise.md) comes from distinct random expression events in the two [genes](../../../../gene.md) and broadens the cloud across that diagonal. Comparable contributions therefore give a noticeably wider, still positively correlated cloud. The two right-hand panels in the preceding original illustration show these two cases.

For matched [fluorescent reporters](../../../../fluorescent-reporter.md) with conditionally independent intrinsic fluctuations and corrected measurement noise,

$$
\eta_{\rm int}^2=\frac12\mathbb E(c-y)^2,\qquad
\eta_{\rm ext}^2=\mathbb E(cy)-1.
$$

The first quantity measures differential variation; the second measures common variation. A clone's successive observations can remain correlated in time, so they need not be independent samples. Shared activation transients should also be separated from the fluctuations of interest.[Science 297 (2002), pp. 1183–1186: dual-reporter discrimination of intrinsic and extrinsic variation](../../../../stochastic-gene-expression-in-a-single-cell-by-michael-b-elowitz-and-others.md)

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
