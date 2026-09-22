<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [linear connection on a manifold](../../../../../affine-connection.md) is a rule $(X,Y)\mapsto\nabla_XY$ for differentiating [vector fields](../../../../../vector-field.md) which is additive, is $C^\infty$-linear in $X$, is real-linear in $Y$, and obeys $\nabla_X(fY)=X(f)Y+f\nabla_XY$. It extends to [covector fields](../../../../../one-form.md) and arbitrary [tensor fields](../../../../../tensor-field.md) by the [Leibniz rule](../../../../../leibniz-rule.md) and compatibility with contraction. In coordinates,

$$
\nabla_aU^d=\partial_aU^d+\Gamma^d{}_{ac}U^c,\qquad
\nabla_a\omega_c=\partial_a\omega_c-\Gamma^d{}_{ac}\omega_d,\qquad
\nabla_af=\partial_af.
$$

This is the [covariant derivative](../../../../../covariant-derivative.md); the [affine connection](../../../../../affine-connection.md) terms correct the changes of the coordinate [basis](../../../../../basis.md). A symmetric [affine connection](../../../../../affine-connection.md) has zero [torsion tensor](../../../../../torsion-tensor.md), $T(X,Y)=\nabla_XY-\nabla_YX-[X,Y]=0$, or $\Gamma^c{}_{ab}=\Gamma^c{}_{ba}$ in a coordinate [basis](../../../../../basis.md). Symmetry does not imply [metric compatibility](../../../../../metric-compatibility.md); no metric is required for this question.

Additivity of each [covariant derivative](../../../../../covariant-derivative.md) immediately gives additivity of $\Delta_{ab}$. Expanding the second derivative of a [tensor product](../../../../../tensor-product.md) gives

$$
\begin{aligned}
\nabla_a\nabla_b(Q\otimes S)={}&(\nabla_a\nabla_bQ)\otimes S+(\nabla_bQ)\otimes\nabla_aS\\
&+(\nabla_aQ)\otimes\nabla_bS+Q\otimes\nabla_a\nabla_bS.
\end{aligned}
$$

Subtract the expression with $a,b$ exchanged. The two mixed terms cancel, proving that the [curvature commutator is a tensor derivation](../../../../../curvature-commutator-is-a-tensor-derivation.md):

$$
\boxed{\Delta_{ab}(Q\otimes S)=(\Delta_{ab}Q)\otimes S+Q\otimes\Delta_{ab}S.}
$$

For a scalar, $\nabla_a\nabla_bf=\partial_a\partial_bf-\Gamma^c{}_{ab}\partial_cf$. Commuting partial derivatives and using the symmetric [affine connection](../../../../../affine-connection.md) gives $\Delta_{ab}f=0$. Consequently $\Delta_{ab}(fU)=f\Delta_{ab}U$: the [commutator](../../../../../commutator.md) is linear over smooth functions, not merely over constant scalars. Write $U=U^ce_c$ in a local [basis](../../../../../basis.md). The [tensor](../../../../../tensor.md)-product rule gives $\Delta_{ab}U=U^c\Delta_{ab}e_c$, showing that its value at a point depends only on $U$ at that point. Thus it defines the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) by

$$
\boxed{\Delta_{ab}U^d=R_{abc}{}^dU^c,\qquad
R_{abc}{}^d=\partial_a\Gamma^d{}_{bc}-\partial_b\Gamma^d{}_{ac}+\Gamma^d{}_{ae}\Gamma^e{}_{bc}-\Gamma^d{}_{be}\Gamma^e{}_{ac}.}
$$

The antisymmetrized second [covariant derivative](../../../../../covariant-derivative.md) is itself tensorial in the derivative indices, so this pointwise map transforms as a [tensor](../../../../../tensor.md). The formula or the defining [commutator](../../../../../commutator.md) gives $R_{abc}{}^d=-R_{bac}{}^d$, hence $R_{abc}{}^d=R_{[ab]c}{}^d$ with normalized antisymmetrization.

Apply the [commutator](../../../../../commutator.md) to the scalar contraction $\omega_cU^c$. Its action vanishes, so

$$
0=(\Delta_{ab}\omega_c)U^c+\omega_cR_{abd}{}^cU^d.
$$

Since $U$ is arbitrary, $\Delta_{ab}\omega_c=-R_{abc}{}^d\omega_d$. Repeated use of the [tensor](../../../../../tensor.md)-product rule gives one plus [curvature](../../../../../curvature.md) action for an upper index and one minus action for each lower index. In particular,

$$
\boxed{\Delta_{ab}S^c{}_{de}=R_{abf}{}^cS^f{}_{de}-R_{abd}{}^fS^c{}_{fe}-R_{abe}{}^fS^c{}_{df}.}
$$

The type notation in the PDF means one contravariant and two covariant indices, not a fractional [tensor](../../../../../tensor.md) order.

For the [first Bianchi identity](../../../../../first-bianchi-identity.md), put $\omega_c=\nabla_cf$ and $H_{bc}=\nabla_b\nabla_cf$. The [symmetric Hessian of a scalar field](../../../../../symmetric-hessian-of-a-scalar-field.md) satisfies $H_{bc}=H_{cb}$. Therefore the six third-derivative terms cancel in

$$
\Delta_{ab}\omega_c+\Delta_{bc}\omega_a+\Delta_{ca}\omega_b
=\nabla_aH_{bc}-\nabla_bH_{ac}+\nabla_bH_{ca}-\nabla_cH_{ba}+\nabla_cH_{ab}-\nabla_aH_{cb}=0.
$$

Substituting the covector [curvature](../../../../../curvature.md) action gives $(R_{abc}{}^d+R_{bca}{}^d+R_{cab}{}^d)\nabla_df=0$. At a chosen point the [gradient](../../../../../gradient.md) of a smooth scalar can be any covector, so

$$
\boxed{R_{abc}{}^d+R_{bca}{}^d+R_{cab}{}^d=0,\qquad R_{[abc]}{}^d=0.}
$$

The second form follows from the already proved first-pair antisymmetry.

For the [second Bianchi identity](../../../../../second-bianchi-identity.md), the same third-derivative cancellation can be organized as an operator identity. On vector-valued components set $D_a=\partial_a+\Gamma_a$, with $(\Gamma_a)^e{}_d=\Gamma^e{}_{ad}$. Although a full second [covariant derivative](../../../../../covariant-derivative.md) includes a term $-\Gamma^f{}_{ab}D_f$ for its lower derivative index, that term cancels on antisymmetrization because the [affine connection](../../../../../affine-connection.md) is symmetric. Thus $[D_b,D_c]=\mathcal R_{bc}$, where $(\mathcal R_{bc})^e{}_d=R_{bcd}{}^e$ acts by multiplication. Expanding the three nested operator [commutators](../../../../../commutator.md) makes all six triple products cancel:

$$
[D_a,[D_b,D_c]]+[D_b,[D_c,D_a]]+[D_c,[D_a,D_b]]=0.
$$

Equivalently, the cyclic sum of $\partial_a\mathcal R_{bc}+[\Gamma_a,\mathcal R_{bc}]$ vanishes. These are the [covariant derivative](../../../../../covariant-derivative.md) terms on the upper and last lower [curvature](../../../../../curvature.md) indices. The two remaining lower indices add $-\Gamma^f{}_{ab}R_{fcd}{}^e-\Gamma^f{}_{ac}R_{bfd}{}^e$. In the cyclic sum these additions cancel in pairs, using $\Gamma^f{}_{ab}=\Gamma^f{}_{ba}$ and $R_{fcd}{}^e=-R_{cfd}{}^e$. Hence the [Bianchi identities from covariant derivative commutators](../../../../../bianchi-identities-from-covariant-derivative-commutators.md) give

$$
\boxed{\nabla_aR_{bcd}{}^e+\nabla_bR_{cad}{}^e+\nabla_cR_{abd}{}^e=0,\qquad\nabla_{[a}R_{bc]d}{}^e=0.}
$$

Both identities here apply to any torsion-free linear [affine connection](../../../../../affine-connection.md); the second derivation does not require choosing a metric [affine connection](../../../../../affine-connection.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
