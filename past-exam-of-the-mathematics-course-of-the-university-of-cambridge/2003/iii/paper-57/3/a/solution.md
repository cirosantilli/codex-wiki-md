<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Poisson manifold](../../../../../../poisson-manifold.md) is a smooth [manifold](../../../../../../topological-manifold.md) $P$ with a bilinear bracket on $C^\infty(P)$ that is antisymmetric, satisfies the [Jacobi identity](../../../../../../jacobi-identity.md) and obeys $\{f,gh\}=\{f,g\}h+g\{f,h\}$. Equivalently it has a [bivector](../../../../../../bivector.md) $\Pi$ defining $\{f,g\}=\Pi(df,dg)$ with vanishing Schouten bracket $[\Pi,\Pi]$; nondegeneracy is not required.

For a [symplectic manifold](../../../../../../symplectic-manifold.md), define the [Hamiltonian vector field](../../../../../../hamiltonian-vector-field.md) by $\iota_{X_f}\omega=df$ and put $\{f,g\}=\omega(X_f,X_g)$. Nondegeneracy gives a unique $X_f$, antisymmetry is inherited from $\omega$, and $d(gh)=g\,dh+h\,dg$ proves the [Leibniz rule](../../../../../../leibniz-rule.md). Moreover $\mathcal L_{X_f}\omega=d\iota_{X_f}\omega+\iota_{X_f}d\omega=0$ by [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md). Since $X_fg=-\{f,g\}$,

$$
\iota_{[X_f,X_g]}\omega=\mathcal L_{X_f}(\iota_{X_g}\omega)=d(X_fg)=-d\{f,g\},
\qquad [X_f,X_g]=-X_{\{f,g\}}.
$$

For completeness, evaluate $d\omega=0$ on $X_f,X_g,X_h$. Its three derivative terms sum to minus the cyclic sum of $\{f,\{g,h\}\}$, and its three bracket terms sum to minus the same cyclic sum, using the displayed identity. Hence that sum is zero. This proves the [Jacobi identity for the Poisson bracket](../../../../../../jacobi-identity-for-the-poisson-bracket.md), not merely the Jacobi identity modulo constants. The inverse of a closed nondegenerate two-form therefore defines a [Poisson manifold](../../../../../../poisson-manifold.md).

The [Symplectic Darboux theorem](../../../../../../darboux-theorem-symplectic-geometry.md) says that near every point of a $2n$-dimensional [symplectic manifold](../../../../../../symplectic-manifold.md) there are coordinates $(q^1,\ldots,q^n,p_1,\ldots,p_n)$ with

$$
\boxed{\omega=\sum_{i=1}^n dq^i\wedge dp_i,\qquad
\{f,g\}=\sum_i\left(\frac{\partial f}{\partial q^i}\frac{\partial g}{\partial p_i}-\frac{\partial f}{\partial p_i}\frac{\partial g}{\partial q^i}\right).}
$$

Thus every symplectic structure has the same local normal form, despite possible global topological differences.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
