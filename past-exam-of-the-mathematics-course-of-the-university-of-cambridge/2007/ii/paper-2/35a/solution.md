<h1 id="35a/solution">Solution</h1>

↑ **Parent:** [35A](../35a.md)

The connection is torsion-free, so on a scalar $\nabla_a\nabla_b\phi=\partial_a\partial_b\phi-\Gamma^c_{ab}\partial_c\phi$ is symmetric in $a,b$. A covector also carries a connection acting on its own index, and commuting derivatives gives curvature, generally nonzero.

Use the curvature convention $[\nabla_a,\nabla_b]v_c=R^d{}_{cab}v_d$, consistent with the identity requested in the PDF. Some texts define the opposite Riemann sign, reversing both formulas. Expanding the prescribed derivative combination of the [Killing equation](../../../../../killing-equation.md) gives

$$
0=\nabla_aS_{bc}+\nabla_bS_{ac}-\nabla_cS_{ab}
=2\nabla_a\nabla_bv_c-[\nabla_a,\nabla_b]v_c+[\nabla_a,\nabla_c]v_b+[\nabla_b,\nabla_c]v_a.
$$

The three commutator terms are $[-R^d{}_{cab}+R^d{}_{bac}+R^d{}_{abc}]v_d=2R^d{}_{abc}v_d$, by antisymmetry in the last two indices and the first [Bianchi identity](../../../../../bianchi-identity.md). Thus

$$
\boxed{\nabla_a\nabla_bv_c=-R^d{}_{abc}v_d.}
$$

In flat Cartesian Minkowski coordinates this says $\partial_a\partial_bv_c=0$. Hence all Killing fields are affine:

$$
\boxed{v^a=a^a+\omega^a{}_b x^b,\qquad \omega_{ab}=-\omega_{ba}.}
$$

The constant term gives four translations and the antisymmetric term six Lorentz generators, rotations and boosts. Conversely every such field satisfies the [Killing equation](../../../../../killing-equation.md).

For the static block metric, time derivatives vanish and $g_{0i}=0$, $g^{00}=-1/f$. The Christoffel formula gives $\Gamma^0_{00}=\Gamma^0_{ij}=0$ and $\Gamma^0_{0i}=\Gamma^0_{i0}=(\partial_if)/(2f)$. The vector $v^a=(1,0,0,0)$ has covector components $v_0=-f$, $v_i=0$. Its only potentially nonzero derivatives are $\nabla_iv_0=-\partial_if/2$ and $\nabla_0v_i=\partial_if/2$; spatial-spatial and time-time derivatives vanish. Their symmetric sums are zero, proving **$\partial_t$ is a [Killing vector field](../../../../../killing-vector-field.md)**.

## ↑ Ancestors (10)

1. [35A](../35a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
