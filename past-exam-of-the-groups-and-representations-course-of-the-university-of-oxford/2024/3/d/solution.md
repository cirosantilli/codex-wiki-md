<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\rho_3(P)=P\otimes P\otimes P$ act on the alternating coefficient [tensor](../../../../tensor.md) $\varphi$, and set

$$
H=\{P\in SO(7):\rho_3(P)\varphi=\varphi\}.
$$

The coefficient convention here is the one in the source's hint; using the usual covariant [pullback](../../../../pullback-category-theory.md) gives the same [stabilizer subgroup](../../../../stabilizer-subgroup.md), since an invertible transformation preserves a [differential form](../../../../differential-form-split.md) if and only if its inverse does. The [identity matrix](../../../../identity-matrix.md) fixes $\varphi$. If $P,Q$ fix it, then $\rho_3(PQ)\varphi=\rho_3(P)\rho_3(Q)\varphi=\varphi$. Multiplying $\rho_3(P)\varphi=\varphi$ by $\rho_3(P^{-1})$ shows that $P^{-1}$ fixes it as well. Thus $H$ is a [subgroup](../../../../subgroup.md) of $SO(7)$. Its defining equations are polynomial, so it is closed and hence a [Matrix Lie group](../../../../matrix-lie-group.md).

For $P(t)=I+tT+O(t^2)\in H$, differentiating $P^TP=I$ gives $T^T=-T$. Differentiating the three factors in $\rho_3(P(t))\varphi=\varphi$ gives

$$
\boxed{\mathfrak h=\left\{T\in\mathfrak{so}(7):
\sum_n\bigl(T_{kn}\varphi_{nlm}+T_{ln}\varphi_{knm}+T_{mn}\varphi_{kln}\bigr)=0
\text{ for all }k,l,m\right\}.}
$$

The [skew-symmetric matrix](../../../../skew-symmetric-matrix.md) condition records the ambient [special orthogonal group](../../../../special-orthogonal-group.md); it must be included when differentiating that group's definition.

These linear conditions are sufficient as well as necessary. On the [tensor product](../../../../tensor-product.md), the infinitesimal action is

$$
D(T)=T\otimes I\otimes I+I\otimes T\otimes I+I\otimes I\otimes T.
$$

Its three terms commute, so $\rho_3(e^{tT})=e^{tD(T)}$. If $D(T)\varphi=0$, every positive power of $D(T)$ annihilates $\varphi$, giving $e^{tD(T)}\varphi=\varphi$. Also $T\in\mathfrak{so}(7)$ implies $e^{tT}\in SO(7)$. Therefore $e^{tT}\in H$, proving the asserted [Lie algebra](../../../../lie-algebra-split.md) description. For the given positive three-form this is the compact [G2](../../../../g2-mathematics.md) [Lie algebra](../../../../lie-algebra-split.md) $\mathfrak g_2$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
