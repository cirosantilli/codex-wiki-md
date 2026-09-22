<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Fix $p\in X$. A linear change of coordinates first identifies $\omega_p$ with the [standard symplectic form](../../../../../standard-symplectic-form.md) $\omega_0$. After shrinking to a star-shaped neighborhood, every

$$
\omega_t=(1-t)\omega_0+t\omega
$$

is nondegenerate. The [Poincaré lemma](../../../../../poincare-lemma.md) gives $\omega-\omega_0=d\sigma$, with $\sigma(p)=0$. Define $X_t$ by $\iota_{X_t}\omega_t=-\sigma$ and let $\phi_t$ be its local flow. [Cartan's magic formula](../../../../../cartan-s-magic-formula.md) gives

$$
\frac d{dt}\phi_t^*\omega_t
=\phi_t^*\bigl(d\sigma+d\iota_{X_t}\omega_t\bigr)=0.
$$

Thus $\phi_1^*\omega=\omega_0$, proving the [Darboux theorem](../../../../../darboux-theorem-symplectic-geometry.md).

For a smooth function $H$ on a closed symplectic manifold, its [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md) is defined by $\iota_{X_H}\omega=-dH$. The same formula gives $\mathcal L_{X_H}\omega=-d^2H=0$, so the [Hamiltonian flow preserves the symplectic form](../../../../../hamiltonian-flow-preserves-the-symplectic-form.md). To move one point to another in a connected $X$, join them by a path, cover the path by finitely many [Darboux charts](../../../../../darboux-chart.md), and in each chart use a cutoff linear Hamiltonian to perform a small translation. Composing these compactly supported Hamiltonian diffeomorphisms proves that **symplectomorphisms act transitively on each connected component**.

In $\mathbb R^2$, every embedded curve is a [Lagrangian submanifold](../../../../../lagrangian-submanifold.md). Let $L_1,L_2$ be circles enclosing different Euclidean areas. A plane symplectomorphism preserves area and carries the bounded complementary component of one circle to that of its image, so no symplectomorphism maps $L_1$ to $L_2$.

The same phenomenon exists in every $\mathbb R^{2n}$. With

$$
\lambda=\frac12\sum_{j=1}^n(x_jdy_j-y_jdx_j),
$$

take the product tori

$$
L_1=S^1(1)^n,
\qquad
L_2=S^1(\sqrt2)^n.
$$

The [Liouville class of a Lagrangian submanifold](../../../../../liouville-class-of-a-lagrangian-submanifold.md) has respective period vectors $\pi(1,\ldots,1)$ and $2\pi(1,\ldots,1)$ on these tori. Every symplectomorphism of $\mathbb R^{2n}$ preserves the Liouville class up to the induced integral change of basis on $H_1(T^n)$, because its pullback changes $\lambda$ only by an exact form. An integral automorphism sends a primitive vector to a primitive vector and therefore cannot send the first period vector to the second. Hence

$$
\boxed{L_1\text{ and }L_2\text{ are compact connected Lagrangians not related by any symplectomorphism}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 146](../../paper-146-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
