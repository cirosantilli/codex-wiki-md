<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define a six-coloring of $\mathbb R^n$ by

$$
c(x)=\left\lfloor3\lVert x\rVert^2\right\rfloor\pmod6.
$$

Let $p,q,r$ be the vertices of a unit [equilateral triangle](../../../../../../equilateral-triangle.md) and let $o$ be its center. Its circumradius is $1/\sqrt3$, and the translation-invariant quadratic identity is

$$
\lVert p\rVert^2+\lVert q\rVert^2+\lVert r\rVert^2-3\lVert o\rVert^2=1.
$$

Suppose all four points had one color $s$. Write

$$
\left\lfloor3\lVert x\rVert^2\right\rfloor=6m_x+s,
\qquad
\theta_x=\left\{3\lVert x\rVert^2\right\}∈[0,1).
$$

Multiplying the quadratic identity by $3$ gives

$$
3=6(m_p+m_q+m_r-3m_o)
+\theta_p+\theta_q+\theta_r-3\theta_o.
$$

The final expression lies strictly between $-3$ and $3$, whereas $3$ is at distance exactly $3$ from the nearest multiple of $6$. This is impossible. The coloring therefore contains no monochromatic copy of the four-point configuration in any dimension $n\geq2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
