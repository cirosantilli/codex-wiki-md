<h1 id="question-4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [steady state](../../../../../../steady-state.md) has $T_s''=0$, so $T_s=a+bx$. The fixed [temperature](../../../../../../temperature-split.md) gives $T_s(0)=T_0$, and [thermal insulation](../../../../../../thermal-insulation.md) gives $T_s'(L)=0$. Thus

$$
\boxed{T_s(x)=T_0.}
$$

Subtracting this [steady state](../../../../../../steady-state.md) produces the homogeneous [mixed boundary conditions](../../../../../../mixed-boundary-condition.md)

$$
\boxed{U_t=\kappa U_{xx},\quad U(0,t)=0,\quad U_x(L,t)=0,\quad
U(x,0)=-\frac{T_0x}{L}.}
$$

The [partial differential equation](../../../../../../partial-differential-equation-split.md) and [boundary conditions](../../../../../../boundary-condition.md) apply for $t>0$. The [initial condition](../../../../../../initial-condition.md) is attained as $t\downarrow0$. Its slope at $x=L$ is $-T_0/L$, so it does not satisfy the insulated-end condition at the instant $t=0$. The resulting [heat equation](../../../../../../heat-equation.md) solution is smooth for $t>0$ and approaches the initial [temperature](../../../../../../temperature-split.md) continuously; its [spatial derivative](../../../../../../spatial-derivative.md) need not be continuous at $(L,0)$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Question 4](../../question-4.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
