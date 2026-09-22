<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In a [coordinate chart](../../../../manifold-chart.md), define the [exterior derivative](../../../../exterior-derivative.md) by

$$
d\left(\sum_Ia_I\,dx^{i_1}\wedge\cdots\wedge dx^{i_r}\right)
=\sum_Ida_I\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_r}.
$$

The chain rule makes this independent of coordinates. It is real linear, increases form degree by one, agrees with the differential on functions, satisfies $d^2=0$, and obeys the [graded Leibniz rule](../../../../graded-leibniz-rule.md)

$$
d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^r\alpha\wedge d\beta.
$$

It also commutes with [pullback](../../../../pullback-category-theory.md) by a [smooth map](../../../../smooth-map-between-manifolds.md). These properties characterize it locally and hence globally.

[de Rham cohomology](../../../../de-rham-cohomology.md) is the quotient of closed forms by exact forms. If $d\alpha=d\beta=0$, Leibniz gives $d(\alpha\wedge\beta)=0$. Changing $\alpha$ to $\alpha+d\eta$ changes the product by $d(\eta\wedge\beta)$; changing $\beta$ to $\beta+d\xi$ changes it by $(-1)^rd(\alpha\wedge\xi)$. Thus

$$
\boxed{[\alpha][\beta]=[\alpha\wedge\beta]}
$$

is independent of representatives. This gives the graded-commutative [de Rham cohomology](../../../../de-rham-cohomology.md) ring.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the lie Groups and Differentiable Manifolds course of the University of Oxford](../../../split.md)
5. [Lie Groups and Differentiable Manifolds course of the University of Oxford](../../../../lie-groups-and-differentiable-manifolds-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
