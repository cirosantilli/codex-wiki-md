<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $A(t)=D_{(x,v)}(X,V)$ along one [characteristic curve](../../../../../../characteristic-curve.md). Differentiating the characteristic equation gives $\dot A=D_zb(t,X,V)A$, $A(0)=I_6$, with $b=(V,F)$. The [Liouville formula for a fundamental matrix](../../../../../../liouville-formula-for-a-fundamental-matrix.md) then gives the [phase-space flow Jacobian](../../../../../../phase-space-flow-jacobian.md)

$$
\boxed{J(t,x,v)=\exp\left(\int_0^t\nabla_v\cdot F(s,X(s),V(s))\,ds\right)}.
$$

Indeed $\operatorname{tr}D_zb=\operatorname{div}_{x,v}(v,F)=\nabla_v\cdot F$, since $v$ is independent of $x$. Differentiation proves $\dot J=(\nabla_v\cdot F)J$. If that [divergence](../../../../../../divergence.md) vanishes, $J(0)=1$ gives $\boxed{J\equiv1}$ and the flow preserves [Lebesgue measure](../../../../../../lebesgue-measure.md) on [phase space](../../../../../../phase-space.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
