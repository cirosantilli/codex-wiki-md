<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Fix the current sign convention by defining the localized variation as $\delta_\epsilon S=-\int d^dx\,(\partial_\mu\epsilon^a)j_a^\mu$. For a first-derivative Lagrangian invariant without a boundary term under constant parameters, this means $j_a^\mu=-\partial\mathcal L/\partial(\partial_\mu\phi)\,t_a\phi$; include the usual improvement term if the constant variation is a total derivative. On solutions, arbitrary compactly supported parameters imply $\partial_\mu j_a^\mu=0$. The [Noether charge](../../../../../noether-charge.md) is $Q_a=\int d^{d-1}x\,j_a^0$ and is conserved if the spatial flux vanishes. This sign convention matches the printed [Ward identity](../../../../../ward-identity.md); reversing the current also reverses the corresponding generator convention.

Assume an invariant regulated [functional measure](../../../../../functional-measure.md), invariant vacuum boundary conditions and no [quantum anomaly](../../../../../anomaly-physics.md). Changing variables in the normalized [path integral](../../../../../path-integral.md) gives $0=\langle\delta_\epsilon X\rangle+i\langle X\delta_\epsilon S\rangle$. Integration by parts then yields

$$
-i\int d^dx\,\epsilon^a(x)\partial_\mu\langle j_a^\mu(x)X\rangle=\langle\delta_\epsilon X\rangle.
$$

For a product of [scalar fields](../../../../../scalar-field.md), the local [Ward identity contact terms](../../../../../ward-identity-contact-terms.md) are

$$
\boxed{-i\partial_\mu\langle j_a^\mu(x)\phi(x_1)\cdots\phi(x_n)\rangle
=\sum_{r=1}^n\delta^d(x-x_r)\langle\phi(x_1)\cdots(t_a\phi)(x_r)\cdots\phi(x_n)\rangle.}
$$

Away from the insertions this is current conservation. Time-ordering or the distributional functional identity supplies the contact terms.

For the gauge theory write $[X,Y]^a=f^{abc}X^bY^c$ and use the [left-acting BRST differential](../../../../../left-acting-brst-differential.md) $s$, with $\delta_\epsilon=\epsilon s$. It obeys the [graded Leibniz rule](../../../../../graded-leibniz-rule.md) and

$$
sA_\mu=D_\mu c,\quad sc=-\tfrac12[c,c],\quad s\bar c=b,\quad sb=0.
$$

Assume the structure constants satisfy the [Jacobi identity](../../../../../jacobi-identity.md) and the dot product is invariant; antisymmetry alone would not be enough. Since $c$ and $D_\mu c$ are odd, their [Lie brackets](../../../../../lie-bracket.md) are symmetric in these two arguments. Consequently

$$
s(D_\mu c)=D_\mu(sc)+[sA_\mu,c]
=-\tfrac12D_\mu[c,c]+[D_\mu c,c]=0.
$$

Also $sF_{\mu\nu}=D_\mu D_\nu c-D_\nu D_\mu c=[F_{\mu\nu},c]$. The [graded Jacobi identity](../../../../../graded-jacobi-identity.md) gives $s[c,c]=0$, so $s^2c=0$; the other three fields have zero second variation immediately. For independent odd parameters, $\delta_{\epsilon'}\delta_\epsilon=-\epsilon'\epsilon s^2=0$. These are off-shell [BRST nilpotence](../../../../../brst-nilpotence.md) identities because the [Nakanishi-Lautrup field](../../../../../nakanishi-lautrup-field.md) $b$ is retained.

The [Yang-Mills theory](../../../../../yang-mills-theory.md) variation is proportional to $F^{\mu\nu}\cdot[F_{\mu\nu},c]=0$. The gauge-fixing variation is $(\partial^\mu b)\cdot D_\mu c$, while the ghost variation is its negative; the $b^2$ term does not vary. Equivalently these terms are $s\Psi$ for the [gauge-fixing fermion](../../../../../gauge-fixing-fermion.md) $\Psi=(\partial^\mu\bar c)\cdot A_\mu+\xi\bar c\cdot b/2$. [BRST nilpotence](../../../../../brst-nilpotence.md) makes this expression invariant. Ghost-number scaling also leaves every term invariant: the ghost and antighost factors carry opposite weights.

Here are the two explicit currents in the same sign convention as the Ward identity. Localizing the even ghost parameter gives coefficient $(\partial_\mu\theta)[\bar c\cdot D^\mu c-(\partial^\mu\bar c)\cdot c]$. Localizing the odd parameter, keeping it on the left, gives coefficient

$$
(\partial_\mu\epsilon)\left[-F^{\mu\nu}\cdot D_\nu c-b\cdot D^\mu c-\frac12(\partial^\mu\bar c)\cdot[c,c]\right].
$$

The last sign comes from moving the odd parameter through the odd antighost derivative. Since the current was defined as minus this coefficient,

$$
\boxed{j_G^\mu=(\partial^\mu\bar c)\cdot c-\bar c\cdot D^\mu c,\qquad
j_B^\mu=F^{\mu\nu}\cdot D_\nu c+b\cdot D^\mu c+\frac12(\partial^\mu\bar c)\cdot[c,c].}
$$

These are the [ghost-number Noether current](../../../../../ghost-number-noether-current.md) and the [BRST current in derivative-b gauge fixing](../../../../../brst-current-in-derivative-b-gauge-fixing.md). If the opposite Noether sign is used, both displayed currents acquire an overall minus sign. Integrating the gauge-fixing term by parts changes the Noether representative by the associated boundary improvement; mixing the two Lagrangian conventions without that improvement gives incorrect signs.

With no BRST anomaly, the conserved odd [BRST charge](../../../../../brst-charge.md) has $Q_B^2=0$. The [BRST cohomology](../../../../../brst-cohomology.md) identifies closed states $Q_B|\psi\rangle=0$ modulo exact states $Q_B|\chi\rangle$. Nilpotence puts every exact state in the closed space. In the usual indefinite gauge-fixed state space, a Hermitian BRST charge makes exact states orthogonal to closed states; the standard no-ghost/positivity assumptions then give a physical [inner product](../../../../../inner-product.md) on the quotient. The physical sector is its ghost-number-zero component,

$$
\boxed{\mathcal H_{\mathrm{phys}}=H^0(Q_B)=\frac{\ker Q_B\cap\mathcal H^0}{Q_B\mathcal H^{-1}}.}
$$

The [ghost number](../../../../../ghost-number.md) assigns $+1$ to $c$, $-1$ to $\bar c$ and zero to gauge and auxiliary fields. Gauge-invariant observables and the chosen vacuum have [ghost number](../../../../../ghost-number.md) zero; unphysical ghost excitations are removed in BRST pairs. Thus physical representatives are expected to satisfy $Q_G|\psi\rangle=0$. This zero-grading selection is part of the physical-state prescription, not a consequence of nilpotence alone.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
