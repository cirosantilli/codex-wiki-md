<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $V=H^0(C,\Omega_C^1)$, of complex dimension $g$, and choose a [symplectic basis](../../../../../symplectic-basis.md) $a_1,\ldots,a_g,b_1,\ldots,b_g$ of $H_1(C,\mathbb Z)$, with $a_i\cdot b_j=\delta_{ij}$. Integration gives a homomorphism

$$
I:H_1(C,\mathbb Z)\longrightarrow V^\vee,\qquad I(\gamma)(\omega)=\int_\gamma\omega.
$$

We first prove both injectivity and discreteness, rather than treating periods as a lattice by definition.

Cut the [compact Riemann surface](../../../../../compact-riemann-surface.md) along this basis to a polygon. For closed one-forms $\omega,\eta$, choose a primitive $F$ of $\omega$ on the cut polygon and apply [Stokes theorem](../../../../../stokes-theorem.md) to $d(F\eta)=\omega\wedge\eta$. Pairing its boundary edges records the jumps of $F$ across the cuts and gives the [Riemann bilinear relations for a compact surface](../../../../../riemann-bilinear-relations-for-a-compact-surface.md):

$$
\int_C\omega\wedge\eta=\sum_i\left(A_i(\omega)B_i(\eta)-B_i(\omega)A_i(\eta)\right),\quad A_i(\omega)=\int_{a_i}\omega,\ B_i(\omega)=\int_{b_i}\omega.
$$

If a [holomorphic differential form](../../../../../holomorphic-differential-form.md) $\omega$ has all $a$-periods zero, take $\eta=\overline\omega$. The right side is zero, while in a holomorphic coordinate, for $\omega=f(z)\,dz$,

$$
\frac{i}{2}\omega\wedge\overline\omega=|f(z)|^2\,dx\wedge dy.
$$

Its integral is strictly positive unless $\omega=0$. Thus the $a$-period map $V\to\mathbb C^g$ is injective, hence an isomorphism. Choose a basis $\omega_1,\ldots,\omega_g$ with $\int_{a_j}\omega_i=\delta_{ij}$, and put $\tau_{ij}=\int_{b_j}\omega_i$. Applying the same boundary identity to $\omega_i,\omega_j$, whose wedge product is zero, gives $\tau_{ij}=\tau_{ji}$. Applying it to $\omega=\sum c_i\omega_i$ and its conjugate gives

$$
\frac{i}{2}\int_C\omega\wedge\overline\omega=c^{\mathsf T}(\operatorname{Im}\tau)\overline c>0\qquad(c\ne0).
$$

Hence $\operatorname{Im}\tau$ is positive definite.

In the dual coordinates, $I(\sum m_ia_i+n_ib_i)=m+\tau n$. The real-linear map $(x,y)\mapsto x+\tau y$ from $\mathbb R^{2g}$ to $\mathbb C^g$ is an isomorphism: taking imaginary parts of a zero gives $(\operatorname{Im}\tau)y=0$, then $y=0$ and $x=0$. Its image of $\mathbb Z^{2g}$ is therefore discrete and cocompact, and no nonzero integral cycle has zero image. Thus

$$
\boxed{I\text{ is injective, with full lattice }\Lambda=\mathbb Z^g+\tau\mathbb Z^g\subset V^\vee.}
$$

The [Abel-Jacobi map of a compact Riemann surface](../../../../../abel-jacobi-map-of-a-compact-riemann-surface.md) sends an effective [complex analytic divisor](../../../../../divisor-on-a-complex-manifold.md) $D=\sum Q_i$ to $\sum_i\int_{P_0}^{Q_i}(\omega_1,\ldots,\omega_g)$ modulo $\Lambda$. Changing a path adds an integral period, so the map is well-defined. For two degree-$d$ [complex analytic divisors](../../../../../divisor-on-a-complex-manifold.md), let $E=D-D'=\sum_P n_PP$, with $\sum n_P=0$, and put

$$
v_i=\sum_P n_P\int_{P_0}^P\omega_i.
$$

We prove that $E$ is principal exactly when $v\in\Lambda$, including the construction of a meromorphic function.

First construct a [differential of the third kind](../../../../../differential-of-the-third-kind.md) $\eta$ with residues $n_P$ at the support of $E$ and no other poles. For the reduced support $S$, the residue exact sequence is

$$
0\longrightarrow K_C\longrightarrow K_C(S)\longrightarrow\bigoplus_{P\in S}\mathbb C_P\longrightarrow0.
$$

On [sheaf cohomology](../../../../../sheaf-cohomology.md), the obstruction to prescribing residues belongs to $H^1(C,K_C)\cong\mathbb C$ by [Serre duality](../../../../../serre-duality.md); its pairing with the constant section of $\mathcal O_C$ is the sum of residues. This follows directly by integrating the local simple-pole terms around the boundary circles. Thus the obstruction is zero because $\sum n_P=0$, and the required $\eta$ exists. Subtract a linear combination of the normalized [holomorphic differential forms](../../../../../holomorphic-differential-form.md) so that all its $a$-periods are zero.

Take its poles and the integration paths inside the same cut polygon. Apply the boundary calculation above to a primitive $F_i(P)=\int_{P_0}^P\omega_i$, removing small circles around the poles of $\eta$. Since $d(F_i\eta)=0$ away from the poles, the paired outer edges contribute $B_i(\eta)$, while the small circles contribute $2\pi i\sum_P n_PF_i(P)$ by the [residue theorem](../../../../../residue-theorem.md). Therefore

$$
\int_{b_i}\eta=2\pi i\,v_i.
$$

The same argument without normalizing $\eta$ gives the useful reciprocity identity

$$
B_i(\eta)-\sum_j\tau_{ij}A_j(\eta)=2\pi i\,v_i.
$$

These identities use compatible cuts and paths; the final conclusions are unchanged by integral periods.

Suppose $v=m+\tau n$ with $m,n\in\mathbb Z^g$. Define

$$
\eta'=\eta-2\pi i\sum_j n_j\omega_j.
$$

Its $a$-periods are $-2\pi i n_i$, and its $b$-periods are $2\pi i m_i$. Around a pole its integral is $2\pi i n_P$. These cycles generate the first [homology group](../../../../../homology-group.md) of the punctured surface, so every period of $\eta'$ belongs to $2\pi i\mathbb Z$. Choosing an auxiliary point $Q$ away from the poles, set

$$
f(P)=\exp\left(\int_Q^P\eta'\right).
$$

It is single-valued away from the poles. Locally $\eta'=n_P\,dt/t+\text{a holomorphic one-form}$, so $f=t^{n_P}$ times a nonvanishing holomorphic function. It extends meromorphically with $\operatorname{div}(f)=E$. This proves sufficiency and explicitly produces the required principal [complex analytic divisor](../../../../../divisor-on-a-complex-manifold.md).

Conversely, if $E=\operatorname{div}(f)$, the meromorphic differential $df/f$ has residues $n_P$ and every period in $2\pi i\mathbb Z$, since each integral counts the winding number of $f$ about zero. Write its $a$-period vector as $2\pi i a$ and its $b$-period vector as $2\pi i b$, with $a,b\in\mathbb Z^g$. The reciprocity identity gives $v=b-\tau a\in\Lambda$. Since $E$ has degree zero, changing the base point cancels in its Abel sum; a base point at the support of $E$ causes no problem, because the Abel integrals use holomorphic forms. We have proved

$$
\boxed{\operatorname{AJ}(D)=\operatorname{AJ}(D')\iff D-D'\text{ is principal}\iff D\sim D'.}
$$

This establishes the [Abel theorem for divisors](../../../../../abel-theorem-for-divisors.md) directly from the period and residue calculations.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
