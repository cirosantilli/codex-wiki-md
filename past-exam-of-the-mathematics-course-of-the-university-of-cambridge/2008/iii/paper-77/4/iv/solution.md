<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A practical family consists of constant-distance [parallel surfaces](../../../../../../parallel-surface.md) and smooth [variable normal offsets](../../../../../../variable-normal-offset.md)

$$
\boxed{P_d(u,v)=P(u,v)+d(u,v)n(u,v),\qquad d(u,v)\text{ represented by a low-degree scalar spline}.}
$$

Constants cover wall thickness, cutter radius and clearance. A scalar [B-spline](../../../../../../b-spline.md) or piecewise [polynomial](../../../../../../polynomial-split.md) displacement field permits thickness variation, local bumps and smooth blending; compact support makes local edits economical. Use the base parameterization or compatible data on its subdivision hierarchy so that evaluating the displacement and its [derivatives](../../../../../../derivative.md) requires only a small local stencil. Choose displacement size and gradients to avoid unintended folds, and trim global self-intersections where the physical application requires an envelope. A constant displacement smaller than the local curvature radii prevents the corresponding local focal singularities, although global clearance still needs a separate check.

When remaining within a polynomial or rational representation is more useful than prescribing an exact distance, a related practical form is $P+\lambda(u,v)(P_u\times P_v)$ with a low-degree scalar field $\lambda$. Its displacement is normal but has magnitude $|\lambda|\lVert P_u\times P_v\rVert$, so it is not a constant-distance [parallel surface](../../../../../../parallel-surface.md). For polynomial $P$ and $\lambda$, it stays polynomial; for rational input it stays rational. More general low-degree vector displacement fields similarly preserve efficient evaluation, while relinquishing the normal-offset condition. These forms make explicit the tradeoff between an exact metric offset, which involves normalization, and an easily represented deformation. **Simple scalar normal-displacement fields are useful and directly evaluable; algebraic displacement fields are useful when representation closure is required.**

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
