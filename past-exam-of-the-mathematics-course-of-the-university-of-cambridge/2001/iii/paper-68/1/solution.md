<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [affine connection](../../../../../affine-connection.md) on the [tangent bundle](../../../../../tangent-bundle.md) of a [smooth manifold](../../../../../smooth-manifold.md) assigns a [vector field](../../../../../vector-field.md) $\nabla_XY$ to two [vector fields](../../../../../vector-field.md), is $\mathbb R$-bilinear, and satisfies

$$
\nabla_{fX}Y=f\nabla_XY,\qquad
\nabla_X(fY)=X(f)Y+f\nabla_XY.
$$

Thus its first slot is [tensorial](../../../../../tensoriality.md) and its second obeys the [Leibniz rule](../../../../../leibniz-rule.md). Its action on [covectors](../../../../../covector.md) is defined by differentiating the pairing, and this extends it to [tensor fields](../../../../../tensor-field.md). A [torsion-free connection](../../../../../torsion-free-connection.md) has $\nabla_XY-\nabla_YX=[X,Y]$.

Assume that $g$ is a smooth [nondegenerate](../../../../../nondegenerate-bilinear-form.md) [metric tensor](../../../../../metric-tensor.md). [Metric compatibility](../../../../../metric-compatibility.md) and a vanishing [torsion tensor](../../../../../torsion-tensor.md) imply the [Koszul formula](../../../../../koszul-formula.md),

$$
2g(\nabla_XY,Z)=Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)
-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
$$

The right-hand side is determined by $g$ and the [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md). Nondegeneracy determines $\nabla_XY$ uniquely; conversely this formula defines an [affine connection](../../../../../affine-connection.md) with both required properties, proving existence as well as uniqueness. In a [coordinate frame](../../../../../coordinate-basis.md) the brackets vanish. Combining the three differentiated [metric tensor](../../../../../metric-tensor.md) identities gives

$$
\boxed{\Gamma^a{}_{bc}
=\frac12g^{ad}(\partial_bg_{dc}+\partial_cg_{db}-\partial_dg_{bc}).}
$$

This is the [Levi-Civita connection](../../../../../levi-civita-connection.md). Positive definiteness is unnecessary: the argument also works for a [pseudo-Riemannian metric](../../../../../pseudo-riemannian-metric.md).

For the other [affine connection](../../../../../affine-connection.md) define $S(X,Y)=\bar\nabla_XY-\nabla_XY$. The [derivative](../../../../../derivative.md) of $f$ cancels between the two [Leibniz rules](../../../../../leibniz-rule.md), so $S$ is $C^\infty$-linear in both slots. The [difference of affine connections is a tensor](../../../../../difference-of-affine-connections-is-a-tensor.md): here $S$ is a section of $TM\otimes T^*M\otimes T^*M$ with components $\bar\Gamma^a{}_{bc}-\Gamma^a{}_{bc}$. Both [affine connections](../../../../../affine-connection.md) are [torsion-free](../../../../../torsion-free-connection.md), so $S(X,Y)=S(Y,X)$.

Agreement of [geodesics](../../../../../geodesic.md) means agreement of their unparametrized curves; different [affine parameters](../../../../../affine-parameter.md) are allowed. For every nonzero tangent vector $v$, existence of a [geodesic](../../../../../geodesic.md) with that initial velocity implies that $S(v,v)$ is parallel to $v$. The [symmetric bilinear diagonal-parallel lemma](../../../../../symmetric-bilinear-diagonal-parallel-lemma.md) now determines $S$. Choose a [basis](../../../../../basis.md) $e_i$ and write $S(e_i,e_i)=\alpha_i e_i$. Applying the parallelism condition to $e_i+e_j$ and $e_i-e_j$ gives

$$
S(e_i,e_j)=\frac12\alpha_j e_i+\frac12\alpha_i e_j.
$$

With $V(e_i)=\alpha_i/2$, [bilinearity](../../../../../bilinearity.md) yields

$$
\boxed{S^a{}_{bc}=\delta^a_bV_c+\delta^a_cV_b
=2\delta^a{}_{(b}V_{c)},\qquad
V_c=\frac{S^a{}_{ac}}{n+1},\quad n=\dim M.}
$$

This is [projective equivalence of affine connections](../../../../../projective-equivalence-of-affine-connections.md). It also covers dimension one. For two [Levi-Civita connections](../../../../../levi-civita-connection.md), the [projective covector from metric volume densities](../../../../../projective-covector-from-metric-volume-densities.md) gives the explicit answer

$$
\boxed{V_c=\frac{1}{2(n+1)}
\partial_c\log\left|\frac{\det\bar g}{\det g}\right|.}
$$

Indeed $\Gamma^a{}_{ac}=\partial_c\log\sqrt{|\det g|}$. The [determinant](../../../../../determinant.md) ratio is a [scalar](../../../../../scalar.md), so this expression is a genuine [covector](../../../../../covector.md), although either [determinant](../../../../../determinant.md) alone is coordinate-dependent. This [determinant](../../../../../determinant.md) expression requires nondegeneracy of $\bar g$; the difference-tensor and earlier [trace](../../../../../matrix-trace.md) formula require only the two torsion-free [affine connections](../../../../../affine-connection.md).

Conversely, the displayed [tensor](../../../../../tensor.md) gives $\bar\nabla_{\dot\gamma}\dot\gamma=2V(\dot\gamma)\dot\gamma$ along an affinely parametrized $\nabla$-[geodesic](../../../../../geodesic.md). Choosing a new parameter $t(\tau)$ satisfying $t''/t'=2V(\dot\gamma)$ removes that tangential acceleration. This [geodesic reparametrization under projective equivalence](../../../../../geodesic-reparametrization-under-projective-equivalence.md) proves sufficiency. If agreement were required with the very same [affine parameter](../../../../../affine-parameter.md), polarization would instead force $S=0$ and $V=0$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
