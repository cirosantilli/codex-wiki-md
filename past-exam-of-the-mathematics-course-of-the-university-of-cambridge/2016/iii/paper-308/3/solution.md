<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**[QCD](../../../../../quantum-chromodynamics.md) supplies the underlying [strong interaction](../../../../../strong-interaction.md); [Skyrmions](../../../../../skyrmion.md) provide a mesonic effective description of [baryons](../../../../../baryon.md), and quantized multi-[Skyrmions](../../../../../skyrmion.md) can model [nuclei](../../../../../atomic-nucleus.md).** These are related descriptions at different scales, not three identical theories.

In [QCD](../../../../../quantum-chromodynamics.md), [quarks](../../../../../quark.md) carry [color charge](../../../../../color-charge.md) and interact through [gluons](../../../../../gluon.md), the gauge fields of the color [special unitary group](../../../../../special-unitary-group.md) $SU(3)$. Its [Lagrangian density](../../../../../lagrangian-density.md) has the form

$$
\mathcal L_{\rm QCD}=-\frac14G^a_{\mu\nu}G^{a\mu\nu}
+\sum_f\overline q_f(i\gamma^\mu D_\mu-m_f)q_f.
$$

[Asymptotic freedom](../../../../../asymptotic-freedom.md) makes short-distance processes accessible through small-coupling expansions, but nuclear scales involve strongly coupled, confined dynamics. Observable [hadrons](../../../../../hadron.md) are color singlets. A [nucleon](../../../../../nucleon.md), either a [proton](../../../../../proton.md) or a [neutron](../../../../../neutron.md), is a [baryon](../../../../../baryon.md) with [baryon number](../../../../../baryon-number.md) one; a [nucleus](../../../../../atomic-nucleus.md) contains $A=Z+N$ such units of [baryon number](../../../../../baryon-number.md). Directly extracting all [nuclear binding energies](../../../../../nuclear-binding-energy.md), spectra and interactions from [QCD](../../../../../quantum-chromodynamics.md) is difficult, motivating low-energy [effective field theories](../../../../../effective-field-theory.md) that preserve its symmetries and relevant degrees of freedom.

For the two light quark flavours, the small-mass limit has approximate [chiral symmetry](../../../../../chiral-symmetry.md) $SU(2)_L\times SU(2)_R$. [Chiral symmetry breaking](../../../../../chiral-symmetry-breaking.md) leaves its vector subgroup $SU(2)_V$, the approximate [isospin](../../../../../isospin.md) symmetry. The three [pions](../../../../../pion.md) are the associated [Goldstone bosons](../../../../../goldstone-boson.md) in the massless limit and [pseudo-Goldstone bosons](../../../../../pseudo-goldstone-boson.md) when the light quark masses are retained. Package these [pions](../../../../../pion.md) into a [special unitary group](../../../../../special-unitary-group.md) field

$$
U(x)=\exp\!\left(\frac{2i\pi_a(x)\sigma_a}{F_\pi}\right),\qquad U\mapsto LUR^\dagger,
$$

where $F_\pi$ is the [pion decay constant](../../../../../pion-decay-constant.md) in this normalization and $\sigma_a$ are the [Pauli matrices](../../../../../pauli-matrices.md). The [nonlinear sigma model](../../../../../nonlinear-sigma-model.md) is the leading two-derivative mesonic theory. The [Skyrme model](../../../../../skyrme-model.md) adds a specific four-derivative stabilizing interaction. One conventional normalization is

$$
\mathcal L_{\rm Sk}=
\frac{F_\pi^2}{16}\operatorname{tr}(\partial_\mu U\,\partial^\mu U^\dagger)
+\frac1{32e^2}\operatorname{tr}([L_\mu,L_\nu][L^\mu,L^\nu])
+\frac{F_\pi^2m_\pi^2}{8}\operatorname{tr}(U-\mathbf1),
\qquad L_\mu=U^\dagger\partial_\mu U.
$$

Here $e$ is a dimensionless model coupling, not electric charge. The last term accounts for a common [pion](../../../../../pion.md) mass and preserves vector [isospin](../../../../../isospin.md). It vanishes in the chiral massless limit. This [effective field theory](../../../../../effective-field-theory.md) uses color-singlet mesonic fields and does not resolve constituent [quarks](../../../../../quark.md) or [gluons](../../../../../gluon.md) inside a [baryon](../../../../../baryon.md).

The condition $U(\mathbf x)\to\mathbf1$ at spatial infinity compactifies physical space to $S^3$. Since $SU(2)$ is itself a three-sphere, the field defines a map $S^3\to S^3$ with integer [topological charge](../../../../../topological-charge.md) in $\pi_3(S^3)=\mathbb Z$. This is identified with the [topological baryon number in the Skyrme model](../../../../../topological-baryon-number-in-the-skyrme-model.md):

$$
\boxed{B=-\frac1{24\pi^2}\int\epsilon_{ijk}\operatorname{tr}(L_iL_jL_k)\,d^3x\in\mathbb Z.}
$$

The associated [topological current](../../../../../topological-current.md) is identically conserved. A single [Skyrmion](../../../../../skyrmion.md) has $B=1$, and a multi-[Skyrmion](../../../../../skyrmion.md) with $B=A>0$ is a candidate intrinsic configuration for an ordinary [nucleus](../../../../../atomic-nucleus.md); negative charge describes antibaryonic sectors. Integer topology prevents a smooth finite-energy unwinding into the [classical vacuum](../../../../../classical-vacuum.md), but it does not by itself guarantee a nonzero-size energy minimum.

The energetic reason for the [Skyrme term](../../../../../skyrme-term.md) is [Derrick scaling](../../../../../derrick-scaling.md). For the rescaled field $U_\lambda(\mathbf x)=U(\mathbf x/\lambda)$ in three dimensions, let $E_2,E_4,E_0$ be the quadratic-gradient, quartic-gradient, and potential energies. Their scale dependence is

$$
E(\lambda)=\lambda E_2+\lambda^{-1}E_4+\lambda^3E_0,
\qquad\boxed{E_2-E_4+3E_0=0\text{ at a stationary solution}.}
$$

The two-derivative [nonlinear sigma model](../../../../../nonlinear-sigma-model.md) alone can lower its static energy by shrinking. The positive quartic [Skyrme term](../../../../../skyrme-term.md) instead grows under shrinking, permitting a balance and a stable soliton size. Without the mass term, this balance gives $E_2=E_4$. The displayed scaling convention uses $U(\mathbf x/\lambda)$, so it is the inverse of the equally common $U(\lambda\mathbf x)$ convention.

The connection with [QCD](../../../../../quantum-chromodynamics.md) is strengthened by [large-Nc baryon scaling](../../../../../large-nc-baryon-scaling.md). Generalize the number of colors to $N_c$ while keeping $g_s^2N_c$ fixed. Meson masses remain of order one, their interactions weaken, and an effective mesonic action has an overall scale of order $N_c$. In the [Skyrme model](../../../../../skyrme-model.md) this corresponds to $F_\pi^2$ and $e^{-2}$ of order $N_c$, so the soliton mass and rotational moment of inertia are also of order $N_c$, whereas rotational level splittings are of order $1/N_c$. These are the expected [baryon](../../../../../baryon.md) scaling properties of large-$N_c$ [QCD](../../../../../quantum-chromodynamics.md). A massive, semiclassical soliton built from meson fields is therefore consistent with the underlying theory, even though physical $N_c=3$ is only a finite value and the simplest [Skyrme model](../../../../../skyrme-model.md) is not uniquely determined by this argument.

To represent a [nucleon](../../../../../nucleon.md), a classical [Skyrmion](../../../../../skyrmion.md) must be quantized. The unit [Skyrmion hedgehog ansatz](../../../../../skyrmion-hedgehog-ansatz.md) ties spatial rotations to [isospin rotations](../../../../../isorotation.md). Its [collective coordinates](../../../../../collective-coordinate-of-a-soliton.md) include its position and orientation; [rotational quantization of a unit Skyrmion](../../../../../rotational-quantization-of-a-unit-skyrmion.md) gives the rotor spectrum

$$
E_J=M+\frac{J(J+1)}{2\Lambda},\qquad J=I,
$$

in units with $\hbar=1$. The [Finkelstein-Rubinstein constraints](../../../../../finkelstein-rubinstein-constraints.md) impose the correct fermionic sign under a nontrivial configuration-space loop. In particular a $2\pi$ spatial rotation acts on a charge-$B$ state by $(-1)^B$ in the physical odd-color theory: odd $B$ admits half-integer [spin](../../../../../spin.md), while even $B$ has integer [spin](../../../../../spin.md). For $B=1$, the lowest allowed $J=I=1/2$ doublet represents the [proton](../../../../../proton.md) and [neutron](../../../../../neutron.md); the $J=I=3/2$ rotor state represents the [Delta baryon](../../../../../delta-baryon.md) resonance. A bosonic [pion](../../../../../pion.md) field can therefore describe fermionic [baryons](../../../../../baryon.md) because the quantum wavefunction carries this nontrivial topological sign.

For [nuclei](../../../../../atomic-nucleus.md), minimize the classical energy in a fixed [baryon number](../../../../../baryon-number.md) sector, then quantize the permitted rotations, [isospin rotations](../../../../../isorotation.md), and relevant vibrations or relative motions. The [toroidal two-Skyrmion](../../../../../toroidal-two-skyrmion.md) has a lowest nuclear state with $J=1,I=0$, identifying it with the [deuteron](../../../../../deuteron.md). The [cubic four-Skyrmion](../../../../../cubic-four-skyrmion.md) has an allowed $J=I=0$ state appropriate to the [alpha particle](../../../../../alpha-particle.md). The [rational map approximation for Skyrmions](../../../../../rational-map-approximation-for-skyrmions.md) makes these intrinsic symmetries easier to construct, while [collective-rotation constraints for a Skyrmion](../../../../../collective-rotation-constraints-for-a-skyrmion.md) select allowed nuclear quantum numbers. A spin-zero state has rotationally invariant laboratory expectation values; a classical cubic intrinsic field should not be interpreted as a fixed cube visible in every orientation. [Collective-coordinate quantization](../../../../../collective-coordinate-quantization.md) restores this distinction between intrinsic shape and a physical quantum state.

The [nuclear force](../../../../../nuclear-force.md) also has a mesonic interpretation. At large separation the tails of [Skyrmions](../../../../../skyrmion.md) are weak [pion](../../../../../pion.md) fields; with nonzero mass their multipole falloff derives from derivatives of the [Yukawa potential](../../../../../yukawa-potential.md). Their interaction depends on relative orientation, and after quantization generates the familiar [spin](../../../../../spin.md)- and [isospin](../../../../../isospin.md)-dependent pion-exchange structure of the [nuclear force](../../../../../nuclear-force.md). Attractive channels allow several unit [Skyrmions](../../../../../skyrmion.md) to form a lower-energy multi-[Skyrmion](../../../../../skyrmion.md). In nuclear language the positive [nuclear binding energy](../../../../../nuclear-binding-energy.md) is the difference between the separated [nucleon](../../../../../nucleon.md) masses and the mass of the quantized bound state, not just a count of topological units.

The limitations remain physical. The simplest [Skyrme model](../../../../../skyrme-model.md) retains only selected terms in a derivative expansion, and finite solitons probe gradients where omitted terms can matter. Its parameters require matching or calibration; predicted binding can be too strong, and masses, radii and spectra are not all fixed correctly by topology. Rotational quantization alone neglects quantum and vibrational corrections, especially when clustering or breakup channels are important. More general mesonic interactions, additional meson fields, and less restrictive classical ansätze can improve the description, but they introduce further low-energy information. **The organizing relation is therefore**

$$
\boxed{\text{QCD}\ \longrightarrow\ \text{chiral mesonic effective theory}
\ \longrightarrow\ \text{topological baryons and quantized multi-Skyrmion nuclear states}.}
$$

It links underlying [quark](../../../../../quark.md) and [gluon](../../../../../gluon.md) dynamics to a geometric, symmetry-based account of [baryons](../../../../../baryon.md) and [nuclei](../../../../../atomic-nucleus.md), while keeping the distinction between an effective approximation and a full derivation from [QCD](../../../../../quantum-chromodynamics.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
