<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $S_{s,t}(y)$ be the position at time $t$ of the [characteristic curve](../../../../../../characteristic-curve.md) satisfying $X(s)=y$ and $\dot X=u(t,X)$. Smooth uniqueness implies $S_{t,s}=S_{s,t}^{-1}$. Differentiating in the initial point gives the [variational equation](../../../../../../variational-equation.md)

$$
\partial_t D_yS_{0,t}
=Du(t,S_{0,t})D_yS_{0,t},\qquad D_yS_{0,0}=I.
$$

The [Liouville formula for a fundamental matrix](../../../../../../liouville-formula-for-a-fundamental-matrix.md), or the derivative formula for a [determinant](../../../../../../determinant.md), therefore gives

$$
\partial_t\det D_yS_{0,t}
=(\operatorname{div}u)(t,S_{0,t})\det D_yS_{0,t}.
$$

Because $u=(-\phi_{x_2},\phi_{x_1})$, the mixed second derivatives cancel and $\operatorname{div}u=0$. The initial [Jacobian determinant](../../../../../../jacobian-determinant.md) is one, so

$$
\boxed{\det D_yS_{0,t}(y)=1.}
$$

Thus this [Hamiltonian flow](../../../../../../hamiltonian-flow.md) preserves planar [Lebesgue measure](../../../../../../lebesgue-measure.md). This calculation assumes smoothness as in the part; a rough-flow conclusion later must be justified by approximation rather than by differentiating a merely continuous velocity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
