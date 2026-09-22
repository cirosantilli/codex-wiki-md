<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take $D_\mu=\partial_\mu+iK_\mu$, with the [Pauli matrices](../../../../../pauli-matrices.md) acting on the [Higgs doublet](../../../../../higgs-field.md). For [electroweak hypercharge](../../../../../hypercharge.md) $Y=1/2$,

$$
K_\mu=\frac g2\tau^aW_\mu^a+\frac{g'}2 B_\mu I_2
=\frac12\begin{pmatrix}gW_\mu^3+g'B_\mu&g(W_\mu^1-iW_\mu^2)\\g(W_\mu^1+iW_\mu^2)&-gW_\mu^3+g'B_\mu\end{pmatrix}.
$$

This specifies every component of the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) for the [electroweak interaction](../../../../../electroweak-interaction.md). Expanding the [gauge-covariant kinetic term](../../../../../gauge-covariant-kinetic-term.md) makes its derivative, trilinear and quartic interactions explicit:

$$
(D_\mu\phi)^\dagger D^\mu\phi=(\partial_\mu\phi)^\dagger\partial^\mu\phi
+i\big[(\partial_\mu\phi)^\dagger K^\mu\phi-\phi^\dagger K_\mu\partial^\mu\phi\big]
+\phi^\dagger K_\mu K^\mu\phi,
$$

where the [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) gives

$$
\phi^\dagger K_\mu K^\mu\phi=
\frac{g^2}{4}W_\mu^aW^{a\mu}\phi^\dagger\phi
+\frac{g'^2}{4}B_\mu B^\mu\phi^\dagger\phi
+\frac{gg'}2W_\mu^aB^\mu\phi^\dagger\tau^a\phi.
$$

The antisymmetric Pauli contribution vanishes because $W_\mu^aW^{b\mu}$ is symmetric in $a,b$. Reversing the sign convention for $D_\mu$ reverses the linear gauge interactions consistently, without changing the masses.

A nonzero [vacuum expectation value](../../../../../vacuum-expectation-value.md) requires $\mu^2<0$. Minimizing the [Higgs potential](../../../../../higgs-field-potential.md) gives $v^2=-\mu^2/\lambda$. By an [gauge transformation](../../../../../gauge-transformation.md) choose

$$
\langle\phi\rangle=\frac1{\sqrt2}\binom0v,\qquad
\phi(x)=\frac1{\sqrt2}\binom0{v+h(x)}
$$

in [unitary gauge](../../../../../unitary-gauge.md). The [electroweak doublet gauge-boson mass matrix](../../../../../electroweak-doublet-gauge-boson-mass-matrix.md) follows by inserting the [vacuum expectation value](../../../../../vacuum-expectation-value.md) in the [gauge-covariant kinetic term](../../../../../gauge-covariant-kinetic-term.md):

$$
\mathcal L_{\mathrm{mass}}=\frac{v^2}{8}\left[g^2\big(W_\mu^1W^{1\mu}+W_\mu^2W^{2\mu}\big)+(gW_\mu^3-g'B_\mu)^2\right].
$$

Define the charged [electroweak gauge bosons](../../../../../electroweak-gauge-boson.md) and the neutral rotation through the [Weinberg angle](../../../../../weinberg-angle.md) by

$$
W_\mu^\pm=\frac{W_\mu^1\mp iW_\mu^2}{\sqrt2},\qquad
s_W=\frac{g'}{\sqrt{g^2+g'^2}},\quad c_W=\frac g{\sqrt{g^2+g'^2}},
$$



$$
Z_\mu=c_WW_\mu^3-s_WB_\mu,\qquad
A_\mu=s_WW_\mu^3+c_WB_\mu,
$$

with inverse $W_\mu^3=c_WZ_\mu+s_WA_\mu$ and $B_\mu=-s_WZ_\mu+c_WA_\mu$. Then

$$
\mathcal L_{\mathrm{mass}}=m_W^2W_\mu^+W^{-\mu}+\frac12m_Z^2 Z_\mu Z^\mu,
\qquad
\boxed{m_W=\frac{gv}{2},\quad m_Z=\frac{v\sqrt{g^2+g'^2}}2,\quad m_A=0.}
$$

The factors differ because $W^+$ and $W^-$ are conjugate fields whereas $Z$ is real. The massless [photon](../../../../../photon.md) corresponds to the unbroken [Lie algebra generator](../../../../../lie-algebra-generator.md) $Q=T_3+Y$, which annihilates $\langle\phi\rangle$. Thus three of the four real [gauge bosons](../../../../../gauge-boson.md) acquire mass, with $m_W=m_Zc_W$. The three would-be [Goldstone bosons](../../../../../goldstone-boson.md) provide their longitudinal polarizations; the remaining scalar $h$ is the [Higgs boson](../../../../../higgs-boson.md).

Introduce the left-handed [lepton](../../../../../lepton.md) doublet $L=(\nu_{eL},e_L)^T$, with $Y_L=-1/2$, and the right-handed singlet $e_R$, with $Y_R=-1$. Use the [chiral projectors](../../../../../chiral-projector.md) $P_L=(1-\gamma^5)/2$ and $P_R=(1+\gamma^5)/2$ in the course's convention. The minimal [Standard Model](../../../../../standard-model-split.md) has no right-handed neutrino. The [gauge-invariant](../../../../../gauge-invariance.md) fermion terms are

$$
\mathcal L_{\ell}=\bar L i\gamma^\mu\left(\partial_\mu+i\frac g2\tau^aW_\mu^a-i\frac{g'}2B_\mu\right)L
+\bar e_Ri\gamma^\mu(\partial_\mu-ig'B_\mu)e_R
-\left(y_e\bar L\phi e_R+y_e^*\bar e_R\phi^\dagger L\right).
$$

The doublet contraction in the [Yukawa interaction](../../../../../yukawa-interaction.md) is a singlet, and its total [hypercharge](../../../../../hypercharge.md) is $+1/2+1/2-1=0$. A bare term $\bar e_Le_R$ would fail [electroweak gauge invariance](../../../../../electroweak-gauge-invariance.md). The [gauge covariant derivatives](../../../../../gauge-covariant-derivative.md) above already give all the requested fermion-gauge couplings. In terms of mass eigenstates, $e=gs_W=g'c_W$ and they become

$$
\mathcal L_{\mathrm{CC}}=-\frac g{\sqrt2}\left(W_\mu^+\bar\nu_{eL}\gamma^\mu e_L+W_\mu^-\bar e_L\gamma^\mu\nu_{eL}\right),\qquad
\mathcal L_{\mathrm{em}}=+eA_\mu\bar e\gamma^\mu e,
$$



$$
\mathcal L_Z=-\frac g{c_W}Z_\mu\left[\frac12\bar\nu_{eL}\gamma^\mu\nu_{eL}
+\left(-\frac12+s_W^2\right)\bar e_L\gamma^\mu e_L+s_W^2\bar e_R\gamma^\mu e_R\right].
$$

Thus the [weak charged current](../../../../../charged-current.md) is chiral and the neutrino has zero [electric charge](../../../../../electric-charge.md). The [gauge-invariant electron Yukawa mass](../../../../../gauge-invariant-electron-yukawa-mass.md) follows from the [Yukawa interaction](../../../../../yukawa-interaction.md) after [electroweak symmetry breaking](../../../../../electroweak-symmetry-breaking.md):

$$
-\frac{v+h}{\sqrt2}\left(y_e\bar e_Le_R+y_e^*\bar e_Re_L\right).
$$

Rephase $e_R$ to make $y_e$ real and positive. It gives

$$
\boxed{m_e=\frac{|y_e|v}{\sqrt2},\qquad \mathcal L_{e,h}=-m_e\bar ee-\frac{m_e}{v}h\bar ee.}
$$

The electron [Dirac mass](../../../../../dirac-mass-term.md) is therefore compatible with the original [gauge symmetry](../../../../../gauge-invariance.md) through the [Higgs mechanism](../../../../../higgs-mechanism.md). The neutrino remains massless in this minimal renormalizable lepton sector.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
