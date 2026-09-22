<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

[inversion in a circle](../../../../../inversion-in-a-circle.md) with center $c$ and radius $r>0$ is $I(z)=c+r^2/(\overline z-\overline c)$, with $c$ and infinity interchanged. It fixes the circle pointwise and reverses complex orientation. Each inversion is fractional-linear in $\overline z$, so composing two eliminates the conjugation and gives $(az+b)/(cz+d)$ with nonzero [determinant](../../../../../determinant.md): a [Möbius transformation](../../../../../mobius-transformation.md).

Translate and rotate two distinct centers to $0,d$, where $d>0$, and let the radii be $r,s$. The composition of inversion in the first circle followed by the second is

$$
T(z)=d+\frac{s^2z}{r^2-dz}.
$$

Its [fixed points](../../../../../fixed-point.md) solve $dz^2-(d^2+r^2-s^2)z+dr^2=0$. The [discriminant](../../../../../discriminant.md) is

$$
\Delta=(d^2-(r+s)^2)(d^2-(r-s)^2).
$$

Disjoint circle boundaries require either $d>r+s$ or $d<|r-s|$, so both factors have the same nonzero sign and $\Delta>0$. There are two distinct [fixed points](../../../../../fixed-point.md) on the line of centers. If the circles are concentric, their radii differ and the composition is $z\mapsto(s^2/r^2)z$, with exactly the two [fixed points](../../../../../fixed-point.md) $0,\infty$. Thus **the composition has two distinct [fixed points](../../../../../fixed-point.md)**, also for nested disjoint circles. Reversing the order inverts the [Möbius transformation](../../../../../mobius-transformation.md) and leaves its [fixed points](../../../../../fixed-point.md) unchanged.

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
