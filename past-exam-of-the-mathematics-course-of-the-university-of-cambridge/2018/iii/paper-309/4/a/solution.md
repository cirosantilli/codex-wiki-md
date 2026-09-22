<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $h_{ab}=\delta g_{ab}$, $h=g^{ab}h_{ab}$, and $h^{ab}=g^{ac}g^{bd}h_{cd}$. Throughout this part use the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) convention printed in the paper. Varying $g^{ac}g_{cb}=\delta^a{}_b$ gives the inverse-metric variation. The [determinant](../../../../../../determinant.md) identity $\delta\log|\det g|=g^{ab}h_{ab}$ gives the [volume form](../../../../../../volume-form.md) variation. Together these are

$$
\boxed{\delta g^{ab}=-h^{ab},\qquad
\delta(d\operatorname{vol}_g)=\frac12h\,d\operatorname{vol}_g.}
$$

In Lorentzian coordinates the latter reads $\delta\sqrt{-g}=\frac12\sqrt{-g}\,h$.

For the connection, vary [metric compatibility](../../../../../../metric-compatibility.md) $\nabla_a g_{bc}=0$:

$$
\nabla_a h_{bc}=g_{dc}\delta\Gamma^d{}_{ab}+g_{bd}\delta\Gamma^d{}_{ac}.
$$

Add the equations with derivatives $a,b$, subtract that with derivative $c$, and use symmetry of the lower indices of the [Levi-Civita connection](../../../../../../levi-civita-connection.md). This gives

$$
\boxed{\delta\Gamma^c{}_{ab}=\frac12g^{cd}
(\nabla_a h_{bd}+\nabla_b h_{ad}-\nabla_d h_{ab}).}
$$

The difference of two connections is a tensor, so this formula is covariant.

Varying the coordinate curvature formula yields the [Palatini identity](../../../../../../palatini-identity.md)

$$
\delta R_{ab}=\nabla_c\delta\Gamma^c{}_{ab}-\nabla_b\delta\Gamma^c{}_{ac}.
$$

The contractions of the connection variation are

$$
g^{ab}\delta\Gamma^c{}_{ab}=\nabla_a h^{ac}-\frac12\nabla^c h,\qquad
\delta\Gamma^c{}_{ac}=\frac12\nabla_a h.
$$

Finally, $\delta R=(\delta g^{ab})R_{ab}+g^{ab}\delta R_{ab}$ gives the [metric variation of scalar curvature](../../../../../../metric-variation-of-scalar-curvature.md):

$$
\boxed{\delta R=-R^{ab}h_{ab}-\nabla^c\nabla_c h+\nabla^a\nabla^b h_{ab},
\qquad\alpha=-1,\quad\beta=1.}
$$

The double divergence may equivalently be written $\nabla_a\nabla_bh^{ab}$: relabeling the contracted dummy indices and using symmetry of $h^{ab}$ gives the same expression. The derivative terms are a [covariant divergence](../../../../../../covariant-divergence.md), useful when varying a curvature-dependent action.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
