<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use $Q=T_3+Y$ and $T_a=\tau_a/2$. For each generation $r=e,\mu,\tau$, the [leptons](../../../../../lepton.md) are

$$
L_r=\binom{\nu_{rL}}{\ell_{rL}}:\ (\mathbf2,-\tfrac12),\qquad R_r=\ell_{rR}:\ (\mathbf1,-1).
$$

Both are color singlets. The conjugate antilepton fields transform in the conjugate representations and have opposite [hypercharge](../../../../../hypercharge.md); they are already included by the conjugate fields in the Lagrangian. The two components of $L_r$ have [electric charges](../../../../../electric-charge.md) $0,-1$, and $R_r$ has charge $-1$. There is no right-handed [neutrino](../../../../../neutrino.md) [representation](../../../../../group-representation.md) in this field content. These assignments use the [electroweak representation and hypercharge table](../../../../../electroweak-representation-and-hypercharge-table.md) in the same [hypercharge](../../../../../hypercharge.md) normalization as the [scalar](../../../../../scalar.md) doublet.

For a doublet of [hypercharge](../../../../../hypercharge.md) $Y$, define

$$
D_\mu=\partial_\mu-ig\frac{\tau_a}{2}A_{a\mu}-ig'YB_\mu.
$$

The $SU(2)$ term is absent for a singlet. Under the local transformation $\psi\mapsto e^{iY\omega}U\psi$, the [gauge fields](../../../../../gauge-field.md) transform so that $D_\mu\psi\mapsto e^{iY\omega}U D_\mu\psi$. Consequently the required [gauge-covariant kinetic terms](../../../../../gauge-covariant-kinetic-term.md) are

$$
\mathcal L_{\rm kin}=\sum_r\bigl(i\bar L_r\gamma^\mu D_\mu L_r+i\bar R_r\gamma^\mu D_\mu R_r\bigr)+(D_\mu\phi)^\dagger D^\mu\phi.
$$

The fields of definite [chirality](../../../../../chirality-physics.md) are defined with $P_{L,R}=(1\mp\gamma_5)/2$. Since $\bar L$ has [hypercharge](../../../../../hypercharge.md) $+1/2$, the [Yukawa interaction](../../../../../yukawa-interaction.md)

$$
\mathcal L_Y=-\sum_{r,s}\bar L_r\phi\,(Y_\ell)_{rs}R_s+\mathrm{h.c.}
$$

is invariant: its [hypercharges](../../../../../hypercharge.md) add to zero, and $\bar L\phi$ contracts the two doublet indices. A bare charged-lepton [mass](../../../../../mass.md) violates these assignments. No renormalizable [neutrino](../../../../../neutrino.md) Yukawa term is available without a right-handed [neutrino](../../../../../neutrino.md). A [gauge-invariant](../../../../../gauge-invariance.md) [scalar potential](../../../../../scalar-potential.md) depending on $\phi^\dagger\phi$ can select the nonzero vacuum, without altering these kinetic and Yukawa constructions.

There is an explicit local [unitary gauge](../../../../../unitary-gauge.md) transformation whenever $r_\phi=(|\phi_1|^2+|\phi_2|^2)^{1/2}\ne0$:

$$
U_\phi=\frac1{r_\phi}\begin{pmatrix}\phi_2&-\phi_1\\\phi_1^*&\phi_2^*\end{pmatrix},\qquad U_\phi^\dagger U_\phi=I,\qquad\det U_\phi=1,\qquad U_\phi\phi=\binom0{r_\phi}.
$$

Thus, with the real field $\rho=\sqrt2r_\phi-v$,

$$
\boxed{\phi=\frac{v+\rho}{\sqrt2}\binom01.}
$$

This proves the [polar coordinates for the electroweak Higgs doublet](../../../../../polar-coordinates-for-the-electroweak-higgs-doublet.md) constructively. The gauge choice is local about the nonzero vacuum; it need not be nonsingular at zeros of the doublet.

The three identical-generation [kinetic terms](../../../../../kinetic-term.md) permit unitary flavor changes. A [singular value decomposition](../../../../../singular-value-decomposition.md) gives $U_L^\dagger Y_\ell U_R=\operatorname{diag}(y_e,y_\mu,y_\tau)$ with $y_r\ge0$. Rotate both components of each left doublet together, and the right singlets independently. In this basis,

$$
\boxed{\mathcal L_Y=-\sum_r m_r\left(1+\frac\rho v\right)\bar\ell_r\ell_r,\qquad m_r=\frac{y_rv}{\sqrt2}.}
$$

The left/right cross terms combine into this [Dirac mass](../../../../../dirac-mass-term.md). Since the [neutrinos](../../../../../neutrino.md) have no [mass](../../../../../mass.md) [matrix](../../../../../matrix.md), their simultaneous left rotation preserves a diagonal [charged current](../../../../../charged-current.md). This is [charged-lepton Yukawa matrix diagonalization](../../../../../charged-lepton-yukawa-matrix-diagonalization.md); the [neutrinos](../../../../../neutrino.md) remain massless in the stated renormalizable model.

The [scalar](../../../../../scalar.md) [kinetic term](../../../../../kinetic-term.md) gives

$$
(D_\mu\phi)^\dagger D^\mu\phi=\frac12(\partial_\mu\rho)^2+\frac{(v+\rho)^2}{8}\bigl[g^2(A_{1\mu}A_1^\mu+A_{2\mu}A_2^\mu)+(gA_{3\mu}-g'B_\mu)^2\bigr].
$$

Introduce $s_W=g'/\sqrt{g^2+g'^2}$ and $c_W=g/\sqrt{g^2+g'^2}$. The combinations $W^+=(A_1-iA_2)/\sqrt2$, $W^-=(W^+)^*$, $Z=c_WA_3-s_WB$ and $A_\gamma=s_WA_3+c_WB$ therefore diagonalize the quadratic terms:

$$
\mathcal L_{\rm mass}=M_W^2W_\mu^+W^{-\mu}+\frac12M_Z^2Z_\mu Z^\mu,\qquad\boxed{M_W=\frac{gv}{2},\quad M_Z=\frac{v\sqrt{g^2+g'^2}}2=\frac{M_W}{c_W},\quad M_\gamma=0.}
$$

The factor $1/2$ applies to the real neutral field, not to the complex charged field. The massless [photon](../../../../../photon.md) corresponds to the unbroken generator $T_3+Y$, which annihilates the vacuum. This gives the [electroweak doublet gauge-boson mass matrix](../../../../../electroweak-doublet-gauge-boson-mass-matrix.md) and its diagonal spectrum.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
