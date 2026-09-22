<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First let $B_{ab}=\nabla_bU_a$ without projection. Commute derivatives on this [covector](../../../../../../../covector.md) and use affine [geodesic](../../../../../../../geodesic.md) motion:

$$
U^c\nabla_cB_{ab}=\nabla_b(U^c\nabla_cU_a)-(\nabla_bU^c)(\nabla_cU_a)-U^cU^dR_{dacb}=-B_{ac}B^c{}_b-R_{cadb}U^cU^d.
$$

The last equality relabels the two contracted null-vector indices. Nullness and affine parametrization give $U^aB_{ab}=0$ and $B_{ab}U^b=0$. Therefore inserting $P$ into the contracted middle index changes no screen-projected quadratic term. Since $\nabla_UP=0$, screen projection proves the [Sachs optical equations](../../../../../../../sachs-optical-equations.md)

$$
\boxed{U\cdot\nabla\widehat B_{ab}=-\widehat B_{ac}\widehat B^c{}_b-\mathcal R_{ab},\qquad\mathcal R_{ab}=P_a{}^eP_b{}^fR_{cedf}U^cU^d.}
$$

The optical tidal [matrix](../../../../../../../matrix.md) $\mathcal R_{ab}$ is symmetric by the [Riemann curvature tensor](../../../../../../../riemann-curvature-tensor.md)'s pair symmetries. Raising one screen index gives the corresponding equation for $\widehat B^a{}_b$.

In terms of the defined optical scalars, the equation is explicitly

$$
\begin{aligned}
U\cdot\nabla\widehat B_{ab}={}&-\frac{\theta^2}{4}P_{ab}-\theta(\widehat\sigma_{ab}+\widehat\omega_{ab})\\
&-\widehat\sigma_{ac}\widehat\sigma^c{}_b-\widehat\omega_{ac}\widehat\omega^c{}_b\\
&-\widehat\sigma_{ac}\widehat\omega^c{}_b-\widehat\omega_{ac}\widehat\sigma^c{}_b-\mathcal R_{ab}.
\end{aligned}
$$

This [matrix](../../../../../../../matrix.md) identity contains the [null expansion](../../../../../../../null-expansion.md), [null shear](../../../../../../../null-shear.md) and [null twist](../../../../../../../null-twist.md) evolution equations as its trace, symmetric trace-free part and antisymmetric part.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 66](../../../../paper-66-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
