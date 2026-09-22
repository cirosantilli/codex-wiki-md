<h1 id="32a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

From $z_j=q_j+ip_j$ and $\bar z_j=q_j-ip_j$, the chain rule gives

$$
\frac{\partial}{\partial q_j}
=\frac{\partial}{\partial z_j}
+\frac{\partial}{\partial\bar z_j},
\qquad
\frac{\partial}{\partial p_j}
=i\frac{\partial}{\partial z_j}
-i\frac{\partial}{\partial\bar z_j}.
$$

Substituting these identities into the canonical [Poisson bracket](../../../../../../poisson-bracket.md) and cancelling the $f_{z_j}g_{z_j}$ and $f_{\bar z_j}g_{\bar z_j}$ terms gives

$$
\boxed{\
\{f,g\}
=-2i\frac{\partial f}{\partial z_j}
\frac{\partial g}{\partial\bar z_j}
+2i\frac{\partial g}{\partial z_j}
\frac{\partial f}{\partial\bar z_j}.\
}
$$

This is the [Poisson bracket in complex canonical coordinates](../../../../../../poisson-bracket-in-complex-canonical-coordinates.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [32A](../../32a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
