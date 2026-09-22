<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

In the [upper half-plane model](../../../../../poincare-half-plane-model.md), [hyperbolic lines](../../../../../hyperbolic-line.md) are vertical Euclidean rays and semicircles centred on the real axis, equivalently circle arcs meeting the real boundary orthogonally. A semicircle with endpoints $r<s$ is mapped to the imaginary axis by

$$
g(z)=\frac{z-r}{s-z},\qquad \text{matrix representative }\frac1{\sqrt{s-r}}\begin{pmatrix}1&-r\\-1&s\end{pmatrix}\in\operatorname{SL}(2,\mathbb R).
$$

Its determinant is one, and its real endpoints map to $0,\infty$. A vertical line $x=a$ is mapped to the imaginary axis by $z\mapsto z-a$. Thus every hyperbolic line can be carried to a fixed one; composing one such map with the inverse of another proves transitivity of $\operatorname{PSL}(2,\mathbb R)$ on the lines.

Reflection in $x=a$ is $R_a(z)=2a-\overline z$. Reflection in the unit semicircle is $R_\circ(z)=1/\overline z$. The latter fixes the semicircle pointwise, is an involution, and preserves the [hyperbolic metric](../../../../../hyperbolic-metric.md) because $|dw|=|dz|/|z|^2$ and $\operatorname{Im}w=\operatorname{Im}z/|z|^2$. The vertical reflection similarly preserves $|dz|/\operatorname{Im}z$. Their composition in the specified order is

$$
\boxed{R_aR_\circ(z)=2a-\frac1z.}
$$

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
