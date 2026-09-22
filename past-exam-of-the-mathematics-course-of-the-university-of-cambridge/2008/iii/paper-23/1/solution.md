<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a real [Lie group](../../../../../lie-group.md) $G$, its [Lie algebra](../../../../../lie-algebra-split.md) is the real [tangent space](../../../../../tangent-space.md) $T_eG$ at the identity. Each tangent vector extends uniquely to a left-invariant vector field, and the [commutator](../../../../../commutator.md) of those fields defines the [Lie bracket](../../../../../lie-bracket.md). For a matrix group this bracket is $[X,Y]=XY-YX$.

For a complex [affine algebraic group](../../../../../linear-algebraic-group.md), the [Lie algebra of an affine algebraic group](../../../../../lie-algebra-of-an-affine-algebraic-group.md) is the complex [Zariski tangent space](../../../../../zariski-tangent-space.md) $T_eG=\operatorname{Hom}_{\mathbb C}(\mathfrak m_e/\mathfrak m_e^2,\mathbb C)$. Its bracket is the [commutator](../../../../../commutator.md) of left-invariant derivations. In a faithful matrix realization, one can compute the [tangent space](../../../../../tangent-space.md) using [dual numbers](../../../../../dual-number.md): $X$ belongs to it exactly when $I+\varepsilon X$ satisfies the group equations modulo $\varepsilon^2$. This is a complex [Lie algebra](../../../../../lie-algebra-split.md), whereas [compact groups](../../../../../compact-group.md) such as $U_n$ and $SU_n$ have real [Lie algebras](../../../../../lie-algebra-split.md).

Differentiate $g^*g=I$ at the identity to get $X^*+X=0$. Conversely $e^{tX}$ is unitary for every skew-Hermitian $X$. Differentiating the [determinant](../../../../../determinant.md) gives $\det(I+tX)=1+t\operatorname{tr}X+O(t^2)$, while $\det e^{tX}=e^{t\operatorname{tr}X}$ proves sufficiency of the trace condition. Finally, $GL_n(\mathbb C)$ is an open subset of all complex matrices, so its [tangent space](../../../../../tangent-space.md) has no linear constraint. Therefore

$$
\boxed{\begin{aligned}
\mathfrak u_n&=\{X\in M_n(\mathbb C):X^*=-X\},\\
\mathfrak{gl}_n(\mathbb C)&=M_n(\mathbb C),\\
\mathfrak{su}_n&=\{X:X^*=-X,\ \operatorname{tr}X=0\},\\
\mathfrak{sl}_n(\mathbb C)&=\{X:\operatorname{tr}X=0\}.
\end{aligned}}
$$

Their dimensions are respectively $n^2,n^2,n^2-1,n^2-1$, with real dimensions for the first and third and complex dimensions for the second and fourth. In every case the [Lie bracket](../../../../../lie-bracket.md) is the matrix [commutator](../../../../../commutator.md).

An irreducible complex [affine algebraic group](../../../../../linear-algebraic-group.md) is connected. It is a [reductive algebraic group](../../../../../reductive-group.md) when its [unipotent radical](../../../../../unipotent-radical.md) $R_u(G)$, the largest connected normal unipotent subgroup, is trivial. This is an algebraic condition; in [characteristic zero](../../../../../characteristic-zero.md) it also implies complete reducibility of finite-dimensional [rational representations](../../../../../rational-representation.md), as proved in Question 2.

Examples are [algebraic tori](../../../../../algebraic-torus.md), $GL_n(\mathbb C)$ and $SL_n(\mathbb C)$, and products of these groups. A diagonal matrix that is unipotent must be the identity, so a torus has no nontrivial unipotent subgroup. For the two matrix groups, let $N$ be a normal unipotent subgroup. The [Kolchin theorem](../../../../../kolchin-theorem.md) supplies a nonzero fixed vector in their standard representation. The subspace fixed by $N$ is invariant under the whole group: for $g\in G$, $n(gv)=g(g^{-1}ng)v=gv$. The standard representation is irreducible, so every vector is fixed by $N$; its faithfulness makes $N$ trivial. A normal unipotent subgroup of a product projects to such a subgroup of each factor, proving the product assertion. By contrast the additive group and a nontrivial upper-unitriangular group are not reductive: their [unipotent radicals](../../../../../unipotent-radical.md) are the whole group.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
