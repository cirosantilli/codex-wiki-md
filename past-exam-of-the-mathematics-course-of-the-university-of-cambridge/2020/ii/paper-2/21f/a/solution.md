<h1 id="21f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $i:Y\hookrightarrow M_f$ be the canonical inclusion and define

$$
r:M_f\longrightarrow Y,\qquad
r(y)=y,\quad r([t,x])=f(x).
$$

This is well-defined because $[0,x]=f(x)$ in the [mapping cylinder](../../../../../../mapping-cylinder.md), and continuity follows from the universal property of the [quotient topology](../../../../../../quotient-topology.md). Clearly $r\circ i=\operatorname{id}_Y$.

Define

$$
H_s(y)=y,\qquad
H_s([t,x])=[(1-s)t,x]
\qquad(0\le s\le1).
$$

The formula respects the gluing relation at $t=0$, so it descends from the disjoint union to a continuous [homotopy](../../../../../../homotopy.md). It satisfies $H_0=\operatorname{id}_{M_f}$ and $H_1=i\circ r$. Thus

$$
\boxed{i:Y\hookrightarrow M_f\text{ is a homotopy equivalence}},
$$

indeed $Y$ is a [deformation retract](../../../../../../deformation-retraction.md) of $M_f$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [21F](../../21f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
