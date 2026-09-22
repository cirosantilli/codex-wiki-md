<h1 id="question-3/d/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

On the unit [circle](../../../../../../../circle.md), the positively oriented unit [tangent vector](../../../../../../../tangent-vector-split.md) is $\mathbf u=(-y,x,0)$, and $|\mathbf u|=1$. Hence $d\mathbf r=\mathbf u\,ds$ and

$$
\oint_C(\psi\mathbf u)\cdot d\mathbf r=\oint_C\psi\,ds.
$$

Since the [scalar field](../../../../../../../scalar-field.md) $\psi$ has no $z$ dependence, the [curl product rule for a scalar field](../../../../../../../curl-product-rule-for-a-scalar-field.md) gives

$$
\begin{aligned}
\nabla\times(\psi\mathbf u)
&=\psi(0,0,2)+(\psi_x,\psi_y,0)\times(-y,x,0)\\
&=(0,0,2\psi+x\psi_x+y\psi_y).
\end{aligned}
$$

On the unit upper [hemisphere](../../../../../../../hemisphere.md) $S_1$, the outward [unit normal vector](../../../../../../../unit-normal.md) is $(x,y,z)$, so its vertical component is $z=\cos\theta$. Applying the [Stokes theorem](../../../../../../../stokes-theorem.md) to the [vector field](../../../../../../../vector-field.md) $\psi\mathbf u$ therefore proves

$$
\boxed{\oint_C\psi\,ds
=\iint_{S_1}\left(2\psi+x\frac{\partial\psi}{\partial x}
+y\frac{\partial\psi}{\partial y}\right)\cos\theta\,dS}.
$$

The smoothness needed here is that $\psi$ extend as a continuously differentiable [scalar field](../../../../../../../scalar-field.md) to a neighbourhood of the projected unit [disk](../../../../../../../disk-mathematics.md). The left side is a scalar [line integral](../../../../../../../line-integral.md) with respect to [arc length](../../../../../../../arc-length.md); the positive [boundary orientation](../../../../../../../boundary-orientation.md) is used when identifying it with the vector [line integral](../../../../../../../line-integral.md).

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [d](../../d.md)
3. [Question 3](../../../question-3.md)
4. [Mathematics V resit](../../../../mathematics-v-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
