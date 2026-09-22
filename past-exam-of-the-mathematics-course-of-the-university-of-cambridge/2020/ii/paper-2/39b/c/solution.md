<h1 id="39b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take a linear combination of the P- and SV-fields from part (b). The rigid boundary condition $\mathbf u=0$ at $z=H$ gives

$$
A\cos(akH)+Bb\cos(bkH)=0,
$$



$$
Aa\sin(akH)-B\sin(bkH)=0.
$$

The conditions at $z=-H$ are the same because the horizontal displacement is even and the vertical displacement is odd. A nonzero pair $(A,B)$ exists exactly when the determinant vanishes:

$$
\cos(akH)\sin(bkH)
+ab\sin(akH)\cos(bkH)=0.
$$

Therefore the [rigid elastic waveguide mode](../../../../../../rigid-elastic-waveguide-mode.md) dispersion relation is

$$
\boxed{
a\tan(akH)
=-\frac{\tan(bkH)}b,
\qquad
a=\sqrt{\frac{c^2}{c_P^2}-1},
\quad
b=\sqrt{\frac{c^2}{c_S^2}-1}
}.
$$

<a id="39b/c/image-dispersion-relation-branches-in-an-elastic-waveguide"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2-elastic-waveguide-dispersion.png)

**[Figure 3](#39b/c/image-dispersion-relation-branches-in-an-elastic-waveguide). Dispersion relation branches in an elastic waveguide**.

As $c$ increases, both $akH$ and $bkH$ increase without bound. The two sides consequently have infinitely many alternating tangent branches and poles. On successive continuity intervals their relative ordering reverses, so the intermediate value theorem gives infinitely many intersections, corresponding to infinitely many propagating waveguide modes.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [39B](../../39b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
