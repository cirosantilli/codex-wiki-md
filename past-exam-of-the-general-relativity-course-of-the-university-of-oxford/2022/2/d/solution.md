<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [metric tensor](../../../../metric-tensor.md) in a basis $\mathbf e_a$ is $g_{ab}=\mathbf e_a\cdot\mathbf e_b$. Differentiating this [inner product](../../../../inner-product-split.md) with the [product rule](../../../../product-rule.md) and using the assumed basis-derivative relation yields

$$
\begin{aligned}
\partial_c g_{ab}
&=(\partial_c\mathbf e_a)\cdot\mathbf e_b
+\mathbf e_a\cdot(\partial_c\mathbf e_b)\\
&=\Gamma^d_{ac}\,\mathbf e_d\cdot\mathbf e_b
+\Gamma^d_{bc}\,\mathbf e_a\cdot\mathbf e_d\\
&=\boxed{\Gamma^d_{ac}g_{db}+\Gamma^d_{bc}g_{ad}.}
\end{aligned}
$$

Thus the coefficients satisfy [metric compatibility](../../../../metric-compatibility.md). For a [coordinate basis](../../../../coordinate-basis.md) with zero [torsion tensor](../../../../torsion-tensor.md), symmetrizing this relation in $a,c$, adding the corresponding two equations and subtracting the third gives

$$
\Gamma^b_{ac}=\frac12g^{bd}
(\partial_a g_{dc}+\partial_c g_{da}-\partial_d g_{ac}).
$$

They are therefore the [Christoffel symbols](../../../../christoffel-symbol.md) of the [Levi-Civita connection](../../../../levi-civita-connection.md). [Metric compatibility](../../../../metric-compatibility.md) by itself does not establish zero [torsion tensor](../../../../torsion-tensor.md); that also uses the [coordinate basis](../../../../coordinate-basis.md) and its commuting coordinate derivatives.

For an embedded curved surface, the stated ambient basis-derivative relation needs a qualification: the [Gauss formula](../../../../gauss-formula.md) is $\partial_c\mathbf e_a=\Gamma^b_{ac}\mathbf e_b+h_{ac}\mathbf n$, where $\mathbf n$ is a [unit normal](../../../../unit-normal.md) and $h_{ac}$ is the [second fundamental form](../../../../second-fundamental-form-split.md). The normal term has zero [inner product](../../../../inner-product-split.md) with each tangent basis vector, so the displayed identity for $\partial_c g_{ab}$ still holds. For a concrete counterexample to dropping that term, on a [two-sphere](../../../../two-sphere.md) one has $\partial_\theta\mathbf e_\theta=-R\mathbf n$, whereas every $\Gamma^b_{\theta\theta}$ is zero. Thus the intrinsic connection describes the tangential projection of the ambient derivative.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
