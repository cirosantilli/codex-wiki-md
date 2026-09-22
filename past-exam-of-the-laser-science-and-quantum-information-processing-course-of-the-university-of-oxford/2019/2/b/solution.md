<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the unfolded propagation convention after reflection. Free-space propagation and a [concave spherical mirror](../../../../concave-spherical-mirror.md) have [matrices](../../../../matrix.md)

$$
T(d)=\begin{pmatrix}1&d\\0&1\end{pmatrix},\qquad
F(R)=\begin{pmatrix}1&0\\-2/R&1\end{pmatrix}.
$$

The [mirror](../../../../mirror.md) is equivalent in this [paraxial](../../../../paraxial-approximation.md) convention to a [thin lens](../../../../thin-lens.md) of [focal length](../../../../focal-length.md) $R/2$. The excursion from the reference plane to [mirror](../../../../mirror.md) 1 and back is

$$
\boxed{S_1=T(L_1)F(R_1)T(L_1)
=\begin{pmatrix}
1-2L_1/R_1&2L_1-2L_1^2/R_1\\
-2/R_1&1-2L_1/R_1
\end{pmatrix}.}
$$

Likewise $S_2=T(L-L_1)F(R_2)T(L-L_1)$. Multiplying $S_2S_1$, or using cyclic invariance of the [trace](../../../../matrix-trace.md) to move the reference plane, gives

$$
\operatorname{tr}M=2-\frac{4L}{R_1}-\frac{4L}{R_2}
+\frac{4L^2}{R_1R_2}
=4g_1g_2-2,
\qquad g_j=1-\frac L{R_j}.
$$

Consequently the strict criterion of [a](../a.md) is

$$
\boxed{0<g_1g_2<1,\qquad g_1=1-L/R_1,\quad g_2=1-L/R_2.}
$$

The [trace](../../../../matrix-trace.md) is independent of $L_1$, as a change of reference plane only conjugates the [round-trip matrix](../../../../ray-transfer-matrix-analysis.md). For the concrete confocal counterexample $R_1=R_2=L$, $L_1=L/2$, each excursion is $\begin{pmatrix}0&L/2\\-2/L&0\end{pmatrix}$ and its square is $-I$. This gives $g_1g_2=0$ and the degenerate boundary exception already explained.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
