<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [torsion tensor](../../../../../../torsion-tensor.md) of an [affine connection](../../../../../../affine-connection.md) is $\mathcal T(X,Y)=\nabla_XY-\nabla_YX-[X,Y]$, where the last term is the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md). A [torsion-free connection](../../../../../../torsion-free-connection.md) has $\mathcal T=0$. Since a [coordinate basis](../../../../../../coordinate-basis.md) commutes, this is equivalent there to $\Gamma^\mu{}_{\nu\rho}=\Gamma^\mu{}_{\rho\nu}$; in a general [basis](../../../../../../basis.md) its commutator must also be included.

The [Levi-Civita connection](../../../../../../levi-civita-connection.md) is the unique [torsion-free connection](../../../../../../torsion-free-connection.md) with [metric compatibility](../../../../../../metric-compatibility.md), $\nabla g=0$. To derive its [Christoffel symbols](../../../../../../christoffel-symbol.md), lower the first index: $\Gamma_{\sigma\nu\rho}=g_{\sigma\mu}\Gamma^\mu{}_{\nu\rho}$. [Metric compatibility](../../../../../../metric-compatibility.md) gives

$$
\partial_\rho g_{\sigma\nu}=\Gamma_{\nu\sigma\rho}+\Gamma_{\sigma\nu\rho}.
$$

Write down this identity with the derivative indices $\rho,\nu,\sigma$, add the first two identities and subtract the third. Symmetry in the last two indices, supplied by the [torsion-free connection](../../../../../../torsion-free-connection.md), cancels all terms except twice $\Gamma_{\sigma\nu\rho}$. Raising the first index yields

$$
\boxed{\Gamma^\mu{}_{\nu\rho}=\frac12g^{\mu\sigma}\bigl(\partial_\rho g_{\sigma\nu}+\partial_\nu g_{\sigma\rho}-\partial_\sigma g_{\nu\rho}\bigr).}
$$

This calculation proves uniqueness. Conversely, these [Christoffel symbols](../../../../../../christoffel-symbol.md) are symmetric in $\nu,\rho$ and satisfy $\nabla g=0$ by substitution, proving existence as well.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
