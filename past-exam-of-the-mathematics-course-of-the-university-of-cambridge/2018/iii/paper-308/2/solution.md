<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [collective coordinate](../../../../../collective-coordinate-of-a-soliton.md) describes a position, orientation, or another parameter of a family of static solitons. For a family $\Phi(\mathbf x;q)$, promote $q$ to a slowly varying $q(t)$ and substitute into the field action. In a scalar theory with unit kinetic coefficient, this gives the [collective-coordinate effective Lagrangian](../../../../../collective-coordinate-effective-lagrangian-for-a-soliton.md)

$$
L_{\rm eff}=\frac12g_{ab}(q)\dot q^a\dot q^b-V(q),\qquad
 g_{ab}=\int\frac{\partial\Phi}{\partial q^a}\cdot\frac{\partial\Phi}{\partial q^b}\,d^dx.
$$

For a [gauge-theory soliton](../../../../../gauge-theory-soliton.md), one also solves the [Gauss law constraint in gauge theory](../../../../../gauss-law-constraint-in-gauge-theory.md) constraint and projects out pure [gauge transformations](../../../../../gauge-transformation.md); arbitrary variations of gauge representatives do not define the physical metric. Tangent vectors to an exactly equal-energy family are [zero modes in field theory](../../../../../zero-mode-in-field-theory.md). If $V=E_0$ is constant, the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) of this [moduli-space approximation](../../../../../moduli-space-approximation-for-solitons.md) are

$$
\ddot q^a+\Gamma^a_{bc}\dot q^b\dot q^c=0,
$$

the [geodesic](../../../../../geodesic.md) equations of its [Riemannian metric](../../../../../riemannian-metric.md). The approximation neglects radiation and deformation modes; it describes motion sufficiently slow that these omitted degrees of freedom remain unexcited to the required accuracy.

In [collective-coordinate quantization](../../../../../collective-coordinate-quantization.md), take the wavefunction measure $\sqrt{\det g}\,d^nq$ and the minimal scalar [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md)

$$
\boxed{\widehat H=-\frac{\hbar^2}{2}\Delta_g+V(q),\qquad
\Delta_g=\frac1{\sqrt{\det g}}\partial_a\left(\sqrt{\det g}\,g^{ab}\partial_b\right).}
$$

The [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) supplies coordinate-invariant kinetic energy. Global identifications and statistics must be imposed on the wavefunctions; the classical metric alone does not choose them. Curvature-ordering terms and loop corrections are additional quantum input.

For the [phi-four kink](../../../../../phi-four-kink.md), use the normalization and profile of Question 1. Substituting $\phi(x,t)=\phi_K(x-X(t))$ gives

$$
L_{
m eff}=-M+\frac12\dot X^2\int(\phi_K')^2dx=-M+\frac12M\dot X^2,
\qquad M=\frac{4c^3}{3}.
$$

The metric is constant because of [translation invariance](../../../../../translation-invariance.md). This proves the [translational dynamics of a phi-four kink](../../../../../translational-dynamics-of-a-phi-four-kink.md): classically the centre moves at constant velocity, and quantum mechanically

$$
\boxed{\widehat H=M-\frac{\hbar^2}{2M}\partial_X^2,\qquad E(p)=M+\frac{p^2}{2M}.}
$$

[Plane waves](../../../../../plane-wave.md) label the continuous translational [momentum](../../../../../momentum.md), with no position-dependent potential. Uniform-motion Lorentz invariance upgrades the dispersion to $\sqrt{M^2+p^2}$; the displayed collective Lagrangian is its small-velocity expansion. Small perturbations also include an internal shape mode and continuum radiation, which this single [collective coordinate](../../../../../collective-coordinate-of-a-soliton.md) omits. The [fluctuation operator of a phi-four kink](../../../../../fluctuation-operator-of-a-phi-four-kink.md) in this normalization is

$$
-\partial_x^2+4c^2-6c^2\operatorname{sech}^2(c(x-X));
$$

the translational eigenfunction has $\omega^2=0$, the shape mode has $\omega^2=3c^2$, and continuum modes in the [spectrum](../../../../../spectrum-functional-analysis.md) start at $\omega^2=4c^2$. Thus the free-coordinate states describe the kink's low translational energies, not its full excitation spectrum or quantum mass correction.

For two [Abelian Higgs vortices](../../../../../nielsen-olesen-vortex.md) at [critical coupling](../../../../../critical-coupling.md), the static energy is $2M_v$ and the [Abelian Higgs vortex moduli space](../../../../../abelian-higgs-vortex-moduli-space.md) has four real dimensions. Let $z_1,z_2$ be their positions, $Z=(z_1+z_2)/2$, and $q=z_1-z_2$. The centre of mass decouples; the relative metric is rotationally symmetric and can be written

$$
ds^2=2M_v|dZ|^2+F(\rho)(d\rho^2+\rho^2d\theta^2),\qquad q=\rho e^{i\theta},\quad\theta\sim\theta+\pi.
$$

At large separation, $F(\rho)\to M_v/2$, recovering two free particles. Although there is no static separation potential, the nonconstant metric produces velocity-dependent interaction. Coincidence is smooth in the [relative coordinate for two identical vortices](../../../../../relative-coordinate-for-two-identical-vortices.md) $w=q^2$, not in the double-valued $q$. Smoothness gives $F(\rho)\sim C\rho^2$ for $C>0$ near zero. A head-on [geodesic](../../../../../geodesic.md) continues through $w=0$ to the opposite real ray, so $q$ changes its line by $\pi/2$: **the vortices scatter through a right angle**. This geometric argument does not require an explicit formula for $F$.

With ordinary bosonic exchange statistics, relative wavefunctions are single-valued in $w$ and smooth at coincidence. In the separated polar coordinate they obey $\Psi(\rho,\theta+\pi)=\Psi(\rho,\theta)$, with even integer angular labels. Their kinetic operator is

$$
\widehat H_{
m rel}=-\frac{\hbar^2}{2F(\rho)}\left[\partial_\rho^2+\frac1\rho\partial_\rho+\frac1{\rho^2}\partial_\theta^2\right].
$$

The apparent singularity at $\rho=0$ must be resolved with the smooth $w$ coordinate and regularity, rather than arbitrary boundary conditions on a punctured cone. The free centre-of-mass motion and the asymptotically free relative geometry give quantum scattering states; a flat static energy does not imply that the metric is flat or that scattering is absent. This is not a prediction of a discrete family of static two-vortex bound separations. The smooth collision geometry is developed in David Tong's [https://arxiv.org/abs/hep-th/0509216.](https://arxiv.org/abs/hep-th/0509216.)

For a [Skyrmion](../../../../../skyrmion.md) of [baryon number](../../../../../baryon-number.md) one, the [Skyrmion hedgehog ansatz](../../../../../skyrmion-hedgehog-ansatz.md) is

$$
U_0(\mathbf x)=\cos f(r)+i\sin f(r)\widehat{\mathbf x}\cdot\boldsymbol\sigma,\qquad f(0)=\pi,\quad f(\infty)=0,
$$

where $\boldsymbol\sigma$ are the [Pauli matrices](../../../../../pauli-matrices.md). Include a centre $\mathbf X$ and an orientation $A\in SU(2)$ through $U=A U_0(\mathbf x-\mathbf X)A^{-1}$. Hedgehog symmetry identifies spatial rotations with opposite internal rotations, so there are three independent orientation coordinates, not six. Since $A$ and $-A$ give the same field, the physical orientation space is $SO(3)$, with [SU(2) group](../../../../../su-2-group.md) as its double cover. Write $A^{-1}\dot A=i\boldsymbol\omega\cdot\boldsymbol\sigma/2$. The leading collective Lagrangian has the form

$$
L_{
m eff}=-M+\frac12M|\dot{\mathbf X}|^2+\frac12\Lambda|\boldsymbol\omega|^2,
$$

where $\Lambda>0$ is the rotational [moment of inertia](../../../../../moment-of-inertia.md) obtained by integrating the profile's field kinetic energy.

For the fermionic quantization appropriate to baryons, the [Finkelstein-Rubinstein constraints](../../../../../finkelstein-rubinstein-constraints.md) on the double cover impose $\Psi(-A)=-\Psi(A)$. In [SU(2) representations](../../../../../representation-theory-of-su-2.md), the central element $-1$ acts by $(-1)^{2j}$, so $j$ must be half-integer. Left and right group actions supply [isospin](../../../../../isospin.md) and [spin angular momentum](../../../../../spin.md); hedgehog symmetry makes their magnitudes equal. The [rotational quantization of a unit Skyrmion](../../../../../rotational-quantization-of-a-unit-skyrmion.md) therefore gives

$$
\boxed{I=J=j=\frac12,\frac32,\ldots,\qquad E_j=M+\frac{j(j+1)\hbar^2}{2\Lambda}.}
$$

The $j=1/2$ level has four spin-isospin states and models the [nucleon](../../../../../nucleon.md) doublet, [proton](../../../../../proton.md) and [neutron](../../../../../neutron.md), each with two spin states. The $j=3/2$ level has sixteen states and models the [Delta baryon](../../../../../delta-baryon.md) quartet, each with four spin states. The rotor predicts a splitting $3\hbar^2/(2\Lambda)$. Without the fermionic sign, single-valued functions on $SO(3)$ would instead allow integer $j$, which is a different quantization. High rotor levels can couple to deformation and pion radiation; this semiclassical approximation does not establish that its entire formal tower consists of stable particles.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
