<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Symplectic Darboux theorem](../../../../../../darboux-theorem-symplectic-geometry.md) says that every point of a $2n$-dimensional [symplectic manifold](../../../../../../symplectic-manifold.md) has local coordinates $(q^1,\ldots,q^n,p_1,\ldots,p_n)$ in which

$$
\boxed{\omega=\sum_{i=1}^n dq^i\wedge dp_i.}
$$

First choose linear coordinates at the point so the form there is standard. The required [symplectic basis](../../../../../../symplectic-basis.md) can be constructed inductively: choose $e,f$ with $\omega(e,f)=1$, split off their span, and repeat on its nondegenerate [symplectic orthogonal complement](../../../../../../symplectic-orthogonal-complement.md). Extend these coordinates to a chart centered at zero.

Let $\omega_0$ be the constant standard form in this chart and $\eta=\omega-\omega_0$. The closed form $\eta$ vanishes at zero. On a small star-shaped ball the radial [Poincaré lemma](../../../../../../poincare-lemma.md) supplies a primitive

$$
\alpha_x(v)=\int_0^1 t\,\eta_{tx}(x,v)\,dt,\qquad d\alpha=\eta.
$$

Since $\eta_0=0$, this primitive is $O(|x|^2)$. The interpolating forms $\omega_t=\omega_0+t\eta$ are nondegenerate on a common smaller ball, because they all agree with $\omega_0$ at zero and $t$ ranges over a compact interval.

Apply the local version of [Moser's trick](../../../../../../moser-s-trick.md): solve $\iota_{X_t}\omega_t=-\alpha$. The [vector fields](../../../../../../vector-field.md) are $O(|x|^2)$ and fix zero. On a sufficiently small ball their flows exist for $0\leq t\leq1$ and remain inside the coordinate chart; the quadratic bound makes their displacement smaller than the available margin. The same pullback calculation gives $f_1^*\omega=\omega_0$. Thus $f_1$ is a local [symplectomorphism](../../../../../../symplectomorphism.md) from the standard ball into $M$, and its inverse supplies the desired [Darboux chart](../../../../../../darboux-chart.md). **There are no local symplectic invariants beyond dimension.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
