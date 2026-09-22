<h1 id="1/b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a fixed [pole](../../../../../../../pole.md) away from the [saddle point](../../../../../../../saddle-point.md), the smooth amplitude there is $(i-z_0)^{-1}$. The [simple-saddle contribution in steepest descent](../../../../../../../simple-saddle-contribution-in-steepest-descent.md) is

$$
J_{\rm sd}(z_0)=\frac{2\sqrt{\pi/k}\,e^{-k}}{i-z_0}\bigl[1+O(k^{-1})\bigr].
$$

The [residue theorem](../../../../../../../residue-theorem.md) supplies an additional contribution precisely when the [contour deformation](../../../../../../../contour-deformation.md) crosses $z_0$. The region swept above the original contour has positive orientation: the original contour from left to right followed by the reversed saddle contour encloses it counterclockwise. Consequently the original integral equals the saddle integral plus the pole contribution:

$$
\boxed{J(z_0)=J_{\rm sd}(z_0)+2\pi i\chi\,e^{k\phi(z_0)}.}
$$

For $|z_0|<1$, an upper-half-plane pole outside the indentation has $\chi=1$, while a lower-half-plane pole has $\chi=0$. The entire upper unit half-disk lies below the saddle [parabola](../../../../../../../parabola.md), so there is no further case inside that half-disk. With a fixed indentation radius $\delta$, a pole inside the upper semicircle, $|z_0|<\delta$, is also below the original contour and has $\chi=0$; real points in the indentation gap are excluded as well. Taking $\delta<|z_0|$ for a fixed nonzero pole gives the usual upper/lower classification. The pole contribution need not always dominate exponentially; its size depends on $\operatorname{Re}\phi(z_0)$, so keeping both terms makes that dependence explicit.

A pole on the original contour requires a stated [Cauchy principal value](../../../../../../../cauchy-principal-value.md) or an indentation prescription. A pole parameter on the negative imaginary [branch cut](../../../../../../../branch-cut.md) still defines the integral: the contour stays on its fixed sheet, and only the denominator uses $z_0$. Such a pole is not crossed, so only $J_{\rm sd}$ is needed and no value of $\sqrt{z_0}$ must be chosen. The residue exponential above is evaluated only when $\chi=1$. At $z_0=0$ the original indentation excludes the singular point, so no additional residue is crossed. These conventions matter before taking any limiting pole position.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 336](../../../../paper-336-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
