<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [cobraided bialgebra](../../../../../../cobraided-bialgebra.md) is a [bialgebra](../../../../../../bialgebra.md) $H$ equipped with a convolution-invertible bilinear form $r:H\otimes H\to k$ satisfying the following identities, in [Sweedler notation](../../../../../../sweedler-notation.md):

$$
\begin{aligned}
r(ab,c)&=\sum r(a,c_{(1)})r(b,c_{(2)}),\\
r(a,bc)&=\sum r(a_{(1)},c)r(a_{(2)},b),\\
\sum r(a_{(1)},b_{(1)})a_{(2)}b_{(2)}
&=\sum b_{(1)}a_{(1)}r(a_{(2)},b_{(2)}),\\
r(1,a)&=r(a,1)=\varepsilon(a).
\end{aligned}
$$

Convolution invertibility means there is $\bar r$ with $\sum r(a_{(1)},b_{(1)})\bar r(a_{(2)},b_{(2)})=\varepsilon(a)\varepsilon(b)$, and likewise with $r,\bar r$ interchanged. This is a [coquasitriangular structure](../../../../../../coquasitriangular-structure.md). On right [comodules](../../../../../../comodule.md) it induces the [braiding](../../../../../../braiding.md)

$$
c(v\otimes w)=\sum w_{(0)}\otimes v_{(0)}r(v_{(1)},w_{(1)}).
$$

The third identity makes this a [comodule](../../../../../../comodule.md) map, the first two give its two hexagon identities, and the convolution inverse gives the inverse [braiding](../../../../../../braiding.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
