<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Quark mixing](../../../../../quark-mixing.md) arises because the up-type and down-type [quark](../../../../../quark.md) [Yukawa matrices](../../../../../yukawa-matrix.md) need not be diagonal in the same [weak interaction](../../../../../weak-interaction.md) basis. In the [Standard Model](../../../../../standard-model-split.md) the three left-handed [quark](../../../../../quark.md) doublets $Q'_L$ transform as $(3,2,1/6)$ under $SU(3)_c\times SU(2)_L\times U(1)_Y$, whereas $u'_R$ and $d'_R$ transform as $(3,1,2/3)$ and $(3,1,-1/3)$. With a [Higgs doublet](../../../../../higgs-field.md) $H$ and its conjugate $\widetilde H=i\sigma^2H^*$, the [gauge-invariant](../../../../../gauge-invariance.md) [Yukawa interaction](../../../../../yukawa-interaction.md) is

$$
\mathcal L_Y=-\bar Q'_L Y_dH d'_R-\bar Q'_L Y_u\widetilde H u'_R+\text{h.c.}
$$

The generation indices are matrix-multiplied. [Electroweak symmetry breaking](../../../../../electroweak-symmetry-breaking.md), $\langle H\rangle=(0,v_H/\sqrt2)^T$, produces $M_u=v_HY_u/\sqrt2$ and $M_d=v_HY_d/\sqrt2$.

Each complex [fermion mass matrix](../../../../../fermion-mass-matrix.md) admits a [biunitary diagonalization](../../../../../singular-value-decomposition.md),

$$
U_{uL}^\dagger M_uU_{uR}=D_u,\qquad U_{dL}^\dagger M_dU_{dR}=D_d,
$$

where the diagonal entries are real nonnegative [quark](../../../../../quark.md) [masses](../../../../../mass.md). Define $u'_L=U_{uL}u_L$ and $d'_L=U_{dL}d_L$, and similarly for right-handed fields. The [kinetic terms](../../../../../kinetic-term.md) retain their canonical form because the transformations are [unitary matrices](../../../../../unitary-matrix.md). However, the [weak charged current](../../../../../charged-current.md) becomes

$$
\mathcal L_{\rm cc}=-\frac{g_2}{\sqrt2}\bar u_L\gamma^\mu Vd_LW^+_\mu+\text{h.c.},\qquad
\boxed{V=U_{uL}^\dagger U_{dL}}.
$$

This [unitary matrix](../../../../../unitary-matrix.md) is the [Cabibbo-Kobayashi-Maskawa matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md). Its entries multiply transitions between up-type and down-type [mass eigenstates](../../../../../mass-eigenstate.md). The minimal [Standard Model](../../../../../standard-model-split.md) has no analogous right-handed [charged weak current](../../../../../charged-current.md).

[Quark mixing](../../../../../quark-mixing.md) does not introduce tree-level [flavor-changing neutral currents](../../../../../flavor-changing-neutral-current.md). [Photon](../../../../../photon.md), [gluon](../../../../../gluon.md) and [weak neutral current](../../../../../neutral-current.md) couplings are proportional to the identity within each fixed-charge [quark](../../../../../quark.md) sector, and $U^\dagger I U=I$. The single [Higgs doublet](../../../../../higgs-field.md) also has diagonal neutral [scalar field](../../../../../scalar-field.md) couplings after the same transformations that diagonalize the [masses](../../../../../mass.md). At higher [loop orders](../../../../../loop-order.md), flavor changes are possible. For example, an $s\to d$ amplitude contains $\sum_iV_{is}^*V_{id}f(m_i^2)$. [Unitarity](../../../../../unitary-operator.md) of the [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md) sets the sum of coefficients to zero, cancelling any [mass](../../../../../mass.md)-independent part. This is the [GIM mechanism](../../../../../gim-mechanism.md); [mass](../../../../../mass.md) splittings leave a suppressed, generally nonzero amplitude.

For $N$ generations a [unitary matrix](../../../../../unitary-matrix.md) has $N^2$ real parameters: $N(N-1)/2$ mixing angles and $N(N+1)/2$ phases. Rephasing the $N$ up-type and $N$ down-type [quark](../../../../../quark.md) fields removes $2N-1$ phases; a common [baryon number](../../../../../baryon-number.md) phase leaves every matrix entry unchanged. Hence the physical numbers are

$$
N_{\rm angles}=\frac{N(N-1)}2,\qquad
N_{\rm weak\ CP\ phases}=\frac{(N-1)(N-2)}2.
$$

Two generations therefore give a real Cabibbo rotation,

$$
V=\begin{pmatrix}\cos\theta_C&\sin\theta_C\\-\sin\theta_C&\cos\theta_C\end{pmatrix},
$$

with [strangeness](../../../../../strangeness.md)-changing charged-current transitions suppressed by $\sin\theta_C$. Three generations have three mixing angles and one irreducible weak [CP](../../../../../cp-symmetry.md) phase. This counting assumes nondegenerate [masses](../../../../../mass.md); degeneracies allow additional basis rotations.

Writing $s_{ij}=\sin\theta_{ij}$ and $c_{ij}=\cos\theta_{ij}$, a standard exact parametrization is

$$
V=\begin{pmatrix}
c_{12}c_{13}&s_{12}c_{13}&s_{13}e^{-i\delta}\\
-s_{12}c_{23}-c_{12}s_{23}s_{13}e^{i\delta}&c_{12}c_{23}-s_{12}s_{23}s_{13}e^{i\delta}&s_{23}c_{13}\\
s_{12}s_{23}-c_{12}c_{23}s_{13}e^{i\delta}&-c_{12}s_{23}-s_{12}c_{23}s_{13}e^{i\delta}&c_{23}c_{13}
\end{pmatrix}.
$$

Complex entries alone do not establish [CP violation](../../../../../cp-violation.md), because [quark](../../../../../quark.md) [quantum field rephasings](../../../../../quantum-field-rephasing.md) can change their phases. For nondegenerate [quark](../../../../../quark.md) [masses](../../../../../mass.md) the weak mixing sector conserves [CP](../../../../../cp-symmetry.md) precisely when a basis makes $V$ real. A useful invariant test is the [Jarlskog invariant](../../../../../jarlskog-invariant.md),

$$
J=\operatorname{Im}(V_{ud}V_{cs}V_{us}^*V_{cd}^*)
=c_{12}c_{23}c_{13}^2s_{12}s_{23}s_{13}\sin\delta.
$$

A nonzero $J$ requires all three mixing angles and a nontrivial phase. If two same-charge [quark](../../../../../quark.md) [masses](../../../../../mass.md) coincide, the additional basis freedom removes the corresponding physical [CP](../../../../../cp-symmetry.md) effect. The possible [QCD theta angle](../../../../../qcd-theta-angle.md) is a separate [CP](../../../../../cp-symmetry.md) parameter, not part of this weak-mixing count.

The [Wolfenstein parametrization](../../../../../wolfenstein-parametrization.md) displays the hierarchy of [quark mixing](../../../../../quark-mixing.md) economically. Put $\lambda_W=s_{12}$, $s_{23}=A\lambda_W^2$, and $s_{13}e^{i\delta}=A\lambda_W^3(\rho+i\eta)$. Expanding the exact matrix gives

$$
V=\begin{pmatrix}
1-\lambda_W^2/2&\lambda_W&A\lambda_W^3(\rho-i\eta)\\
-\lambda_W&1-\lambda_W^2/2&A\lambda_W^2\\
A\lambda_W^3(1-\rho-i\eta)&-A\lambda_W^2&1
\end{pmatrix}+O(\lambda_W^4).
$$

The observed pattern is predominantly diagonal, with $1$-$2$ mixing largest and $2$-$3$, $1$-$3$ mixing successively suppressed. The expansion implies $J\simeq A^2\lambda_W^6\eta$. The truncated matrix must not be treated as an exactly [unitary matrix](../../../../../unitary-matrix.md).

Column [orthogonality](../../../../../orthogonal-vectors.md) gives

$$
V_{ud}V_{ub}^*+V_{cd}V_{cb}^*+V_{td}V_{tb}^*=0.
$$

The three complex numbers form a [CKM unitarity triangle](../../../../../ckm-unitarity-triangle.md), with area $|J|/2$. Dividing by $-V_{cd}V_{cb}^*$ puts its vertices at $0$, $1$ and $\bar\rho+i\bar\eta$, where $\bar\rho+i\bar\eta=-V_{ud}V_{ub}^*/(V_{cd}V_{cb}^*)$. The barred parameters include higher-order corrections to the Wolfenstein parameters. Comparing independent measurements of its sides and angles tests both [quark mixing](../../../../../quark-mixing.md) and the absence of additional flavor dynamics.

Semileptonic [decay rates](../../../../../decay-width.md) determine magnitudes of [CKM](../../../../../cabibbo-kobayashi-maskawa-matrix.md) entries through factors $|V_{ij}|^2$ once hadronic [matrix elements](../../../../../matrix-element.md) are controlled. Neutral [kaon](../../../../../kaon.md) and neutral B-[meson](../../../../../meson.md) mixing constrain products of entries through weak box [scattering amplitudes](../../../../../scattering-amplitude.md). [CP](../../../../../cp-symmetry.md) asymmetries probe their invariant relative phases, with [kaon](../../../../../kaon.md) mixing providing indirect [CP violation](../../../../../cp-violation.md) and [decay amplitudes](../../../../../decay-amplitude.md) providing direct [CP violation](../../../../../cp-violation.md). These processes complement tests of the [unitarity](../../../../../unitary-operator.md) constraints on rows and columns. **The minimal three-generation [Standard Model](../../../../../standard-model-split.md) describes weak [quark mixing](../../../../../quark-mixing.md) by a [unitary matrix](../../../../../unitary-matrix.md) with three angles and one physical [CP](../../../../../cp-symmetry.md) phase; it does not predict the [Yukawa couplings](../../../../../yukawa-interaction.md) or their hierarchy.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
