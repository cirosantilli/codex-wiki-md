<h1 id="26i/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The original perimeter is

$$
P(\Omega)=\int_{x_0}^{x_1}
\left(\sqrt{1+u_+'(x)^2}+\sqrt{1+u_-'(x)^2}\right)dx.
$$

The two boundary graphs of the symmetrized domain are $\pm h/2$, so

$$
P(S_L(\Omega))
=\int_{x_0}^{x_1}\sqrt{4+(u_+'-u_-')^2}\,dx.
$$

Apply the triangle inequality in $\mathbb R^2$ to the vectors

$$
(1,u_+'),\qquad(1,-u_-').
$$

It gives pointwise

$$
\sqrt{1+u_+'{}^2}+\sqrt{1+u_-'{}^2}
\geq\sqrt{4+(u_+'-u_-')^2}.
$$

After integration,

$$
\boxed{P(S_L(\Omega))\leq P(\Omega).}
$$

Equality in the Euclidean triangle inequality holds exactly when the two displayed vectors are nonnegative scalar multiples. Their first coordinates are both one, so this means

$$
u_+'=-u_-'.
$$

Equality of perimeters therefore holds exactly when $u_+(x)+u_-(x)=c$ is constant. In that case the midpoint of every vertical chord lies on $y=c/2$, and $\Omega$ has the horizontal line $y=c/2$, parallel to $L$, as an axis of symmetry. The converse is immediate.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [26I](../../../26i.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
