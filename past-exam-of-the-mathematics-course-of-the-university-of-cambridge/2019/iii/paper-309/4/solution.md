<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the torsion-free [Levi-Civita connection](../../../../../levi-civita-connection.md), cyclically summing the displayed coordinate expression and using $\Gamma^a{}_{bc}=\Gamma^a{}_{cb}$ gives the algebraic [first Bianchi identity](../../../../../first-bianchi-identity.md)

$$
\boxed{R^a{}_{bcd}+R^a{}_{cdb}+R^a{}_{dbc}=0}.
$$

Apply the [Jacobi identity](../../../../../jacobi-identity.md) to three covariant-derivative commutators, or differentiate the coordinate formula in [normal coordinates](../../../../../normal-coordinates.md). The third-derivative terms and the derivatives of quadratic connection terms cancel cyclically, giving the differential [second Bianchi identity](../../../../../second-bianchi-identity.md)

$$
\boxed{\nabla_eR^a{}_{bcd}
+\nabla_cR^a{}_{bde}
+\nabla_dR^a{}_{bec}=0}.
$$

Contracting the first and third curvature indices and then contracting once more yields

$$
\nabla^aR_{ab}-\frac12\nabla_bR=0,
$$

or the [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md)

$$
\boxed{\nabla^aG_{ab}=0}.
$$

For the metric variation $h_{ab}=\delta g_{ab}$,

$$
\delta\sqrt{-g}=\frac12\sqrt{-g}\,h,
$$

while the two double-divergence terms in the supplied [metric variation of scalar curvature](../../../../../metric-variation-of-scalar-curvature.md) become a boundary term after [integration by parts for tensor fields](../../../../../integration-by-parts-for-tensor-fields.md). The [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md) therefore contributes $G_{ab}+\Lambda g_{ab}$. Varying the [Proca action](../../../../../proca-action.md) with respect to the metric gives the [Proca stress-energy tensor](../../../../../proca-stress-energy-tensor.md), and the full [Einstein-Proca theory](../../../../../einstein-proca-theory.md) equation is

$$
\boxed{
R_{ab}-\frac12Rg_{ab}+\Lambda g_{ab}
=8\pi\left[
F_{ac}F_b{}^c-\frac14g_{ab}F_{cd}F^{cd}
+m^2A_aA_b-\frac12m^2g_{ab}A_cA^c
\right]}.
$$

Since $\delta F_{ab}=2\nabla_{[a}\delta A_{b]}$, variation with respect to $A_b$ and one [integration by parts](../../../../../integration-by-parts.md) give the covariant [Proca equation](../../../../../proca-equation.md)

$$
\boxed{\nabla_aF^{ab}-m^2A^b=0}.
$$

Taking its [covariant divergence](../../../../../covariant-divergence.md) gives

$$
m^2\nabla_bA^b=\nabla_b\nabla_aF^{ab}
=\frac12[\nabla_b,\nabla_a]F^{ab}=0,
$$

because the resulting contractions pair the symmetric [Ricci tensor](../../../../../ricci-tensor.md) with the antisymmetric [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md). Since $m\ne0$, the [Lorenz constraint in Proca theory](../../../../../lorenz-constraint-in-proca-theory.md) follows:

$$
\boxed{\nabla_aA^a=0}.
$$

Moreover, $F=dA$ and $d^2=0$, so the [Electromagnetic Bianchi identity](../../../../../electromagnetic-bianchi-identity.md) is

$$
\boxed{\nabla_aF_{bc}+\nabla_bF_{ca}+\nabla_cF_{ab}=0}.
$$

Finally, use that identity to differentiate the matter tensor. The result groups naturally as

$$
\nabla^aT_{ab}
=F_b{}^c\left(\nabla^aF_{ac}-m^2A_c\right)
+m^2A_b\nabla_aA^a.
$$

Both terms vanish by the [Proca equation](../../../../../proca-equation.md) and its [Lorenz constraint in Proca theory](../../../../../lorenz-constraint-in-proca-theory.md). Thus $\nabla^aT_{ab}=0$, exactly as required by the [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) applied to the [Einstein field equations](../../../../../einstein-field-equations.md). The vector equation is therefore consistent with the gravitational equation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 309](../../paper-309-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
