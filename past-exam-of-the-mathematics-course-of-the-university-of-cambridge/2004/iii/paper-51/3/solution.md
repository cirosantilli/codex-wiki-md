<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $F_+=(F+*F)/2$ and $F_-=(F-*F)/2$, using the oriented [Euclidean metric](../../../../../euclidean-metric.md). For a [self-dual two-form](../../../../../self-dual-differential-form.md) $\omega$,

$$
\omega\wedge F=\langle\omega,*F\rangle\,\mathrm{vol}
=\langle\omega,F_+\rangle\,\mathrm{vol}.
$$

Apply this componentwise in the [Lie algebra](../../../../../lie-algebra-split.md). Since the three $\omega_i$ span the self-dual subspace, their vanishing wedges force $F_+=0$. Thus **$*F=-F$**. The [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) is $D_AF=0$, so $D_A*F=-D_AF=0$, the Euclidean [Yang-Mills equations](../../../../../yang-mills-equations.md). This proves the implication locally; finite action would additionally be needed to call the solution an [instanton](../../../../../instanton.md).

Use the complex orientation for $w=x^1+ix^2$ and $z=x^3+ix^4$. The real and imaginary parts of $dw\wedge dz$, and $i(dw\wedge d\bar w+dz\wedge d\bar z)$, span the [self-dual two-forms](../../../../../self-dual-differential-form.md). Accordingly the three [gauge curvature](../../../../../gauge-field-strength.md) equations are

$$
F_{wz}=0,\qquad F_{\bar w\bar z}=0,\qquad F_{w\bar w}+F_{z\bar z}=0.
$$

For a [spectral parameter](../../../../../spectral-parameter.md) $\lambda\in\mathbb{CP}^1$, consider the [Lax pair](../../../../../lax-pair.md)

$$
\boxed{(D_w-\lambda D_{\bar z})\Psi=0,\qquad(D_z+\lambda D_{\bar w})\Psi=0.}
$$

Their [commutator](../../../../../commutator.md) is

$$
[D_w-\lambda D_{\bar z},D_z+\lambda D_{\bar w}]
=F_{wz}+\lambda(F_{w\bar w}+F_{z\bar z})+\lambda^2F_{\bar w\bar z}.
$$

It vanishes for every $\lambda$ exactly when all three coefficients vanish. The derivative directions $\partial_w-\lambda\partial_{\bar z}$ and $\partial_z+\lambda\partial_{\bar w}$ are mutually orthogonal [null vectors](../../../../../null-vector.md) for the complexified metric. Flatness on the corresponding two-planes makes the linear parallel-transport equations locally compatible. Conversely compatibility for an invertible fundamental [matrix](../../../../../matrix.md) $\Psi$ forces the [commutator](../../../../../commutator.md) to vanish; a single zero solution would not establish it. This is the [Euclidean complex-coordinate anti-self-dual Lax pair](../../../../../euclidean-complex-coordinate-anti-self-dual-lax-pair.md).

For an [Abelian](../../../../../abelian-group.md) [U(1) connection](../../../../../u-1-connection.md), all [commutators](../../../../../commutator.md) of the connection components vanish, and the [gauge curvature](../../../../../gauge-field-strength.md) equations therefore read

$$
\boxed{\begin{aligned}
\partial_w A_z-\partial_z A_w&=0,\\
\partial_{\bar w}A_{\bar z}-\partial_{\bar z}A_{\bar w}&=0,\\
\partial_zA_{\bar z}-\partial_{\bar z}A_z
+\partial_wA_{\bar w}-\partial_{\bar w}A_w&=0.
\end{aligned}}
$$

Locally the first two equations say that $A^{1,0}$ is $\partial$-closed and $A^{0,1}$ is $\bar\partial$-closed. The [Dolbeault-Poincaré lemma](../../../../../dolbeault-poincare-lemma.md), and its [complex conjugate](../../../../../complex-conjugate.md), give scalar functions $u,v$ with

$$
A=\partial u+\bar\partial v.
$$

Substituting in the third equation gives

$$
(v-u)_{z\bar z}+(v-u)_{w\bar w}=0.
$$

In a complex [gauge transformation](../../../../../gauge-transformation.md), use $g=e^{-u}$ and the derivative-plus-connection convention $A\mapsto A+g^{-1}dg$. Then

$$
\boxed{A'=\bar\partial f,\qquad f=v-u,\qquad f_{z\bar z}+f_{w\bar w}=0.}
$$

This is the scalar [Laplace equation](../../../../../laplace-equation.md), since for the stated metric $\Delta=2(\partial_z\partial_{\bar z}+\partial_w\partial_{\bar w})$. The complex [gauge transformation](../../../../../gauge-transformation.md) need not remain in $U(1)$.

A reduction using only a [unitary](../../../../../unitary-connection.md) [gauge transformation](../../../../../gauge-transformation.md) is also available. Since $A$ is [anti-Hermitian](../../../../../skew-hermitian-matrix.md), $A_{\bar w}=-\overline{A_w}$ and $A_{\bar z}=-\overline{A_z}$, so the potential for the barred components can be chosen as $v=-\bar u$. Write $u=p+iq$ with real $p,q$. Then $A=\partial p-\bar\partial p+i\,dq$, and $g=e^{-iq}$ removes the last term. With $f=-2p$ this gives

$$
\boxed{A'=\frac12(\bar\partial f-\partial f),\qquad f\text{ real},\qquad f_{z\bar z}+f_{w\bar w}=0.}
$$

Its [gauge curvature](../../../../../gauge-field-strength.md) is $\partial\bar\partial f$. Thus the [Abelian anti-self-dual connections from harmonic scalar potentials](../../../../../abelian-anti-self-dual-connections-from-harmonic-scalar-potentials.md) reduction is local and does not require silently enlarging the real gauge group.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
