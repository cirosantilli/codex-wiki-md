<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose representatives $\lambda_1,\ldots,\lambda_r$ as in part (b). We use the [symplectic centralizer decomposition](../../../../symplectic-centralizer-decomposition.md)

$$
\boxed{C_{\mathfrak{sp}(V)}(\mathfrak a)\cong\mathfrak{sp}(V_0)\oplus\bigoplus_{i=1}^r\mathfrak{gl}(V_{\lambda_i}).}
$$

To prove it, a [linear map](../../../../linear-map.md) commuting with every $a\in\mathfrak a$ must preserve every [weight space](../../../../weight-space.md): if $v\in V_\lambda$, then $a(Tv)=T(av)=\lambda(a)Tv$. Conversely, preserving the [weight spaces](../../../../weight-space.md) makes a [linear map](../../../../linear-map.md) commute with the scalar action of every $a$ on each space.

On $V_0$, the [symplectic Lie algebra](../../../../symplectic-lie-algebra.md) condition says exactly that the restriction belongs to $\mathfrak{sp}(V_0)$. On $V_{\lambda_i}\oplus V_{-\lambda_i}$, use the [perfect pairing](../../../../perfect-pairing.md) from part (b) to identify $V_{-\lambda_i}$ with the [dual space](../../../../dual-space-split.md) $V_{\lambda_i}^*$. The action $A_i$ on $V_{\lambda_i}$ can be arbitrary, but its action on $V_{-\lambda_i}$ must be $-A_i^*$, where $A_i^*$ is the [dual map](../../../../transpose-of-a-linear-map.md). Indeed,

$$
\omega(A_iv,w)+\omega(v,B_iw)=0\quad\text{for all }v,w
$$

determines $B_i=-A_i^*$ uniquely. There are no additional conditions between different pairs because $\omega$ vanishes between different pairs. Every choice of these blocks therefore gives an element of the [centralizer of a Lie subalgebra](../../../../centralizer-of-a-lie-subalgebra.md). The block correspondence preserves [Lie brackets](../../../../lie-bracket.md), proving the claimed [direct sum of Lie algebras](../../../../direct-sum-of-lie-algebras.md).

The [general linear Lie algebra](../../../../general-linear-lie-algebra.md) $\mathfrak{gl}_m(k)$ is an [abelian Lie algebra](../../../../abelian-lie-algebra.md) exactly when $m\leq1$: for $m\geq2$, the [matrix units](../../../../matrix-unit.md) satisfy $[E_{11},E_{12}]=E_{12}\ne0$. A nonzero [symplectic vector space](../../../../symplectic-vector-space.md) has a [symplectic basis](../../../../symplectic-basis.md) and contains a two-dimensional [symplectic subspace](../../../../symplectic-subspace.md). The [symplectic Lie algebra](../../../../symplectic-lie-algebra.md) acting on that plane, extended by zero on its [symplectic orthogonal complement](../../../../symplectic-orthogonal-complement.md), contains the [matrices](../../../../matrix.md) $H=\operatorname{diag}(1,-1)$ and $E=E_{12}$ with $[H,E]=2E\ne0$. Thus $\mathfrak{sp}(V_0)$ is an [abelian Lie algebra](../../../../abelian-lie-algebra.md) exactly when $V_0=0$.

Since different summands in a [direct sum of Lie algebras](../../../../direct-sum-of-lie-algebras.md) commute, we obtain the precise criterion

$$
\boxed{C_{\mathfrak{sp}(V)}(\mathfrak a)\text{ is abelian}\iff\begin{gathered}V_0=0,\\\dim V_\lambda=1\quad(0\ne\lambda\in\Psi(\mathfrak a)).\end{gathered}}
$$

Equivalently, there are $2n$ distinct nonzero [weights of a representation](../../../../weight-of-a-representation.md), each with a one-dimensional [weight space](../../../../weight-space.md). The condition concerns multiplicities in the [defining representation](../../../../defining-representation-of-a-matrix-lie-algebra.md); it does not assert that $\dim\mathfrak a=n$ for every such $\mathfrak a$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the lie algebras course of Part C of the mathematics course of the University of Oxford](../../../split.md)
5. [Lie algebras course of Part C of the mathematics course of the University of Oxford](../../../../lie-algebras-course-of-part-c-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
