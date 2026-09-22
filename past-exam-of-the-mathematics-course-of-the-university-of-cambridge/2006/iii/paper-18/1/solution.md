<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $X$ be a connected [compact Riemann surface](../../../../../compact-riemann-surface.md) of [geometric genus](../../../../../geometric-genus.md) $g$, equivalently a [smooth projective curve](../../../../../smooth-projective-curve.md) over $\mathbb C$, and put $V=H^0(X,K_X)$. Choose a [symplectic basis](../../../../../symplectic-basis.md) $a_1,\ldots,a_g,b_1,\ldots,b_g$ of $H_1(X,\mathbb Z)$ with $a_i\cdot b_j=\delta_{ij}$. For a closed [differential form](../../../../../differential-form-split.md) $\alpha$, write $A_i(\alpha)=\int_{a_i}\alpha$ and $B_i(\alpha)=\int_{b_i}\alpha$. The underlying bilinear identity is

$$
\int_X\alpha\wedge\beta=\sum_{i=1}^g\bigl(A_i(\alpha)B_i(\beta)-B_i(\alpha)A_i(\beta)\bigr).
$$

It holds for any two smooth closed one-forms. In particular, the [Riemann bilinear relations](../../../../../riemann-bilinear-relations-for-a-compact-surface.md) for [holomorphic differential forms](../../../../../holomorphic-differential-form.md) are

$$
\sum_i\bigl(A_i(\omega)B_i(\eta)-B_i(\omega)A_i(\eta)\bigr)=0,
\qquad
 i\sum_i\bigl(A_i(\omega)\overline{B_i(\omega)}-B_i(\omega)\overline{A_i(\omega)}\bigr)>0
$$

for $\omega,\eta\in V$ and $\omega\ne0$ in the inequality. The inequality fixes the orientation and the sign convention.

To prove the identity, cut $X$ along the [symplectic basis](../../../../../symplectic-basis.md) to a fundamental polygon $P$. On $P$, a closed one-form $\alpha$ has a primitive $F$. The [Stokes theorem](../../../../../stokes-theorem.md) gives

$$
\int_P\alpha\wedge\beta=\int_{\partial P}F\beta.
$$

Opposite copies of each cut have opposite orientations, while their values of $F$ differ by the corresponding period of $\alpha$. Pairing those edges therefore leaves $A_i(\alpha)\int_{b_i}\beta-B_i(\alpha)\int_{a_i}\beta$ for the $i$th handle. Summing proves the identity. The same calculation can be made with a small disk about the polygon's vertices removed; its extra boundary terms tend to zero, so the vertices cause no additional term.

For [holomorphic differential forms](../../../../../holomorphic-differential-form.md) $\omega,\eta$, their [wedge product of differential forms](../../../../../wedge-product-of-differential-forms.md) vanishes: locally both are multiples of $dz$. This proves the first relation. If $\omega=f(z)\,dz$ and $z=x+iy$, then

$$
i\omega\wedge\overline\omega=2|f(z)|^2\,dx\wedge dy.
$$

A nonzero [holomorphic differential form](../../../../../holomorphic-differential-form.md) is nonzero on an open set, so the integral is strictly positive. Applying the identity to $\omega,\overline\omega$ proves the second relation.

These relations first prove that the map $V\to\mathbb C^g$ taking $a$-periods is injective: if every $A_i(\omega)$ vanishes, the positive integral just computed would vanish. Since $\dim V=g$ by the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md), it is an isomorphism. Consequently there is a unique [basis](../../../../../basis.md) $\omega_1,\ldots,\omega_g$ with $\int_{a_j}\omega_i=\delta_{ij}$. Set $\tau_{ij}=\int_{b_j}\omega_i$. The first relation gives $\tau_{ij}=\tau_{ji}$, and the second gives, for any nonzero column $c$,

$$
i\int_X\left(\sum_i c_i\omega_i\right)\wedge\overline{\left(\sum_i c_i\omega_i\right)}=2c^t(\operatorname{Im}\tau)\overline c>0.
$$

Thus **the normalized [period matrix of a complex torus](../../../../../period-matrix-of-a-complex-torus.md) is symmetric and has positive-definite imaginary part**:

$$
\boxed{\tau^t=\tau,\qquad Y=\operatorname{Im}\tau>0.}
$$

The integration map sends a cycle $\gamma$ to the functional $\omega\mapsto\int_\gamma\omega$ in $V^*$. In the normalized [basis](../../../../../basis.md) its image is the [period lattice](../../../../../period-lattice.md)

$$
\Lambda=\mathbb Z^g+\tau\mathbb Z^g.
$$

Indeed, the real-linear map $(x,y)\mapsto x+\tau y$ from $\mathbb R^{2g}$ to $\mathbb C^g$ is an isomorphism: its imaginary part is $Yy$, and $Y$ is invertible. Its image of $\mathbb Z^{2g}$ is therefore discrete and has compact quotient. This proves that

$$
\boxed{\operatorname{Jac}(X)=V^*/\Lambda\cong\mathbb C^g/(\mathbb Z^g+\tau\mathbb Z^g)}
$$

is a well-defined $g$-dimensional [complex torus](../../../../../complex-torus.md), rather than merely a quotient by an arbitrary subgroup.

The relations also provide its canonical principal [polarization of a complex torus](../../../../../polarization-of-a-complex-torus.md). With the convention that a [Hermitian form](../../../../../hermitian-form.md) is conjugate-linear in its first argument, put $H(z,w)=\overline z^{,t}Y^{-1}w$ and $E=\operatorname{Im}H$. Symmetry of $\tau$ gives

$$
E(m+\tau n,m'+\tau n')=m^tn'-n^tm',\qquad E(v,iv)=H(v,v)>0.
$$

In particular $E$ is integral and unimodular on $\Lambda$, and it is compatible with the complex structure. These are exactly the positivity and integrality conditions for a [Riemann form on a complex torus](../../../../../riemann-form-on-a-complex-torus.md); they make the [complex torus](../../../../../complex-torus.md) a [Jacobian variety](../../../../../jacobian-variety.md) with a principal [polarization of a complex torus](../../../../../polarization-of-a-complex-torus.md). If instead one uses a first-argument-linear [Hermitian form](../../../../../hermitian-form.md), the same alternating form is $-\operatorname{Im}H$. Changing the [symplectic basis](../../../../../symplectic-basis.md) changes the coordinates but not this polarized quotient. For $g=0$, $V=0$ and the [Jacobian variety](../../../../../jacobian-variety.md) is a point.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
