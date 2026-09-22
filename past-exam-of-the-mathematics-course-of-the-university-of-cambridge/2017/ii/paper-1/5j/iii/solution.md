<h1 id="5j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The dashed curves are contours of constant [Cook's distance](../../../../../../cook-s-distance.md), labelled 0.5 and 1, in the plot of standardized residual against [regression leverage](../../../../../../regression-leverage.md). Writing $h_{ii}$ for the diagonal of the [hat matrix](../../../../../../hat-matrix.md), $s^2$ for the residual [variance](../../../../../../variance-split.md) estimate, and $p=8$ for the number of fitted coefficients,

$$
r_i=\frac{e_i}{s\sqrt{1-h_{ii}}},\qquad
\boxed{D_i=\frac{r_i^2}{p}\frac{h_{ii}}{1-h_{ii}}}.
$$

Thus a contour $D_i=d$ has $r_i=\pm\sqrt{dp(1-h_{ii})/h_{ii}}$. On the actual PDF plot, observation 579 has leverage about 0.084 and standardized residual about $-8$, lying beyond the $D=0.5$ contour and below $D=1$ in influence magnitude, approximately $D\simeq0.7$ to $0.8$ from the plotted coordinates. It is unusually light relative to its fitted log-weight and potentially influential because deleting it can materially change fitted coefficients. It warrants checking, not automatic deletion. The solid smooth red curve is distinct from the dashed [Cook's distance](../../../../../../cook-s-distance.md) contours.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5J](../../5j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
