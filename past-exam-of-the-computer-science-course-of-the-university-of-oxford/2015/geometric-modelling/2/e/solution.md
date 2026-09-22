<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Rotating the geometry through $180^\circ$ sends every [point](../../../../../point-geometry.md) $p$ to $-p$. To start the extension at the origin, also reverse the parameter:

$$
E(t)=-F(1-t),\qquad
\boxed{E(t)=(2t^2,\,-2t+2t^2),\quad 0\le t\le1.}
$$

Then $E(0)=(0,0)=F(1)$ and $E(1)=(2,0)$. Merely using $-F(t)$ would trace the same rotated image toward the origin, instead of away from the join.

The reversed and rotated [de Boor points](../../../../../de-boor-point.md) are $-D_2,-D_1,-D_0$, namely $(0,1),(0,-1),(4,1)$. The first two are already $D_1,D_2$, so there is only one new [de Boor point](../../../../../de-boor-point.md), $\boxed{D_3=(4,1)}$. Using the same uniform basis [matrix](../../../../../matrix.md),

$$
\boxed{E(t)=\frac12[t^2\ t\ 1]
\begin{pmatrix}1&-2&1\\-2&2&0\\1&1&0\end{pmatrix}
\begin{pmatrix}0&1\\0&-1\\4&1\end{pmatrix}.}
$$

Equivalently, the [Bézier curve](../../../../../bezier-curve.md) handles are $C=(0,0)$, $-B=(0,-1)$ and $-A=(2,0)$, which gives the same [polynomials](../../../../../polynomial-split.md) immediately.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Geometric modelling](../../../geometric-modelling-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
