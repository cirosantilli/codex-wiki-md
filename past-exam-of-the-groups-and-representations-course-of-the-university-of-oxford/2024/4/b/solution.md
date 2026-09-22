<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First prove surjectivity. For any $A\in U(n)$, its [determinant](../../../../determinant.md) has modulus one. Choose $z\in U(1)$ with $z^n=\det A$ and define $U=z^{-1}A$. Then $U^\dagger U=I$ and $\det U=z^{-n}\det A=1$, so $A=f(z,U)$.

Next, $f(z,U)=I$ is equivalent to $U=z^{-1}I$. This lies in $SU(n)$ precisely when $z^n=1$. Therefore the [kernel of a group homomorphism](../../../../kernel-of-a-group-homomorphism.md) is the central [cyclic group](../../../../cyclic-group.md)

$$
\boxed{\ker f=\{(\zeta^k,\zeta^{-k}I_n):k=0,\ldots,n-1\}\cong\mathbb Z_n,
\qquad\zeta=e^{2\pi i/n}.}
$$

Its generator is $(\zeta,\zeta^{-1}I_n)$, which has order $n$. The inverse phases in the two factors are essential: this is an explicitly embedded [subgroup](../../../../subgroup.md), not a quotient by scalar [matrices](../../../../matrix.md) in just one factor. The [first isomorphism theorem](../../../../first-isomorphism-theorem.md) now gives

$$
\boxed{U(n)\cong\bigl(U(1)\times SU(n)\bigr)/\mathbb Z_n.}
$$

This also holds as a [Lie group isomorphism](../../../../lie-group-isomorphism.md): the induced map is smooth and a continuous bijection from a compact [quotient space](../../../../quotient-topological-space.md) to the Hausdorff [unitary group](../../../../unitary-group.md), and its differential is the [Lie algebra isomorphism](../../../../lie-algebra-isomorphism.md) $(it,X)\mapsto itI+X$. For $n=1$ the [kernel of a group homomorphism](../../../../kernel-of-a-group-homomorphism.md) is trivial, consistently with $SU(1)=\{1\}$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
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
