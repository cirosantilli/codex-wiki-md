# Paper 44

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper44.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper44.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use [natural units](../../../physics.md#natural-units) and the [Minkowski metric](../../../special-relativity.md#minkowski-metric) $g=\operatorname{diag}(1,-1,-1,-1)$. The [Lorentz group](../../../special-relativity.md#lorentz-group) is

$$
G=O(1,3)=\{L\in GL(4,\mathbb R):L^TgL=g\}.
$$

Write a transformation near the identity as $L=I+\Omega+O(\Omega^2)$. The defining relation gives $\Omega^Tg+g\Omega=0$, so $\omega_{\mu\nu}=g_{\mu\rho}\Omega^\rho{}_\nu$ is antisymmetric. Choose

$$
(M^{\rho\sigma})^\mu{}_\nu
=g^{\rho\mu}\delta^\sigma_\nu-g^{\sigma\mu}\delta^\rho_\nu,
\qquad
\Omega=\frac12\omega_{\rho\sigma}M^{\rho\sigma}.
$$

There are $\binom42=\boxed{6}$ independent real parameters: three spatial rotations and three [Lorentz boosts](../../../special-relativity.md#lorentz-boost). Differentiating $(e^{t\Omega})^Tg e^{t\Omega}$ with respect to $t$ shows it is constant and equals $g$. Thus exponentiating these infinitesimal generators gives [Lorentz transformations](../../../special-relativity.md#lorentz-transformation) connected to the identity. The component they generate is the [Proper orthochronous Lorentz group](../../../special-relativity.md#proper-orthochronous-lorentz-group) $G_0=SO^+(1,3)$, characterized by $\det L=1$ and $L^0{}_0>0$.

The local exponential calculation alone establishes products of exponentials. The single-exponential assertion also holds here. Use the [Lorentz spinor double cover](../../../special-relativity.md#lorentz-spinor-double-cover) $SL(2,\mathbb C)\to SO^+(1,3)$, obtained by acting on $X=x^0I+x^a\sigma_a$ as $X\mapsto AXA^\dagger$. Its [determinant](../../../linear-algebra.md#determinant) is the Minkowski norm. A lift $A$ with distinct eigenvalues $\lambda,\lambda^{-1}$ is diagonalizable and has a traceless logarithm with eigenvalues $z,-z$, where $e^z=\lambda$. With repeated eigenvalues, choose between $A$ and $-A$ so that the lift is $I+N$ with $N^2=0$; its traceless logarithm is $N$. Since the two signs have the same Lorentz image, exponentiating the differential of the covering map proves [every proper orthochronous Lorentz transformation is an exponential](../../../special-relativity.md#every-proper-orthochronous-lorentz-transformation-is-an-exponential):

$$
\boxed{L=\exp\left(\frac12\omega_{\rho\sigma}M^{\rho\sigma}\right).}
$$

It is not a global assertion about the disconnected improper components of $G$.

For [Dirac spinors](../../../relativistic-quantum-field.md#dirac-spinor), choose [gamma matrices](../../../algebra.md#gamma-matrices) satisfying the [Clifford algebra](../../../algebra.md#clifford-algebra) $\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu}I$ and set

$$
\Sigma^{\rho\sigma}=\frac14[\gamma^\rho,\gamma^\sigma],
\qquad S=\exp\left(\frac12\omega_{\rho\sigma}\Sigma^{\rho\sigma}\right).
$$

The Clifford relations give

$$
[\Sigma^{\rho\sigma},\gamma^\mu]
=g^{\sigma\mu}\gamma^\rho-g^{\rho\mu}\gamma^\sigma.
$$

They also give the stipulated Lorentz [commutator](../../../lie-algebra.md#commutator) with every $M$ replaced by $\Sigma$: commute $\Sigma$ through the two gamma factors defining the other generator and collect the four terms. Consequently this is a representation of the [Lie algebra of the Lorentz group](../../../special-relativity.md#lie-algebra-of-the-lorentz-group), and exponentiation yields

$$
S^{-1}\gamma^\mu S=L^\mu{}_\nu\gamma^\nu,\qquad
\psi'(x')=S\psi(x),\quad x'=Lx.
$$

The [Dirac adjoint](../../../relativistic-quantum-field.md#dirac-adjoint) $\bar\psi=\psi^\dagger\gamma^0$ transforms as $\bar\psi'=\bar\psi S^{-1}$, since $S^\dagger\gamma^0S=\gamma^0$.

There is a global qualification: a spatial rotation through $2\pi$ gives $S=-I$, while its Lorentz [matrix](../../../vector-space.md#matrix) is $I$. Thus **[Dirac spinors](../../../relativistic-quantum-field.md#dirac-spinor) form an ordinary representation of the double cover, and a double-valued representation of $G_0$**, rather than a single-valued linear representation of $G_0$ itself. [Fermion bilinears](../../../relativistic-quantum-field.md#fermion-bilinear) are unaffected by this sign.

For a [scalar field](../../../quantum-field-theory.md#scalar-field), $\phi'(x')=\phi(x)$ and its derivative transforms as a covector. A [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) must have all Lorentz indices contracted into scalars using invariant tensors; arbitrary scalar potentials are allowed. For example the kinetic contraction and a potential $V(\phi)$ are invariant. Lorentz invariance by itself does not restrict the potential to quartic order: that restriction would be an additional four-dimensional power-counting requirement.

Define $\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3$. It commutes with all $\Sigma^{\rho\sigma}$, so the [axial current](../../../relativistic-quantum-field.md#axial-current) $j_5^\mu=\bar\psi\gamma^\mu\gamma^5\psi$ transforms as a vector under $G_0$. Hence **all three proposed contractions are invariant under $G_0$**. If invariance under parity or the full improper [Lorentz group](../../../special-relativity.md#lorentz-group) is also required, the distinction is:

$$
\begin{array}{c|c|c}
\text{operator}&G_0&\text{parity, for ordinary scalar }\phi\\ \hline
\partial_\mu\phi\,\partial^\mu\phi&\text{invariant}&\text{even}\\
\partial_\mu\phi\,j_5^\mu&\text{invariant}&\text{odd}\\
j_{5\mu}j_5^\mu&\text{invariant}&\text{even}.
\end{array}
$$

The [axial current](../../../relativistic-quantum-field.md#axial-current) is a [pseudovector](../../../vector-space.md#pseudovector): under an improper [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) it has the extra [determinant](../../../linear-algebra.md#determinant) sign. The mixed derivative–axial contraction is therefore a [pseudoscalar](../../../quantum-mechanics.md#pseudoscalar), while the square of the [axial current](../../../relativistic-quantum-field.md#axial-current) has two cancelling signs. If $\phi$ is itself a [pseudoscalar](../../../quantum-mechanics.md#pseudoscalar), its derivative supplies the second sign and the mixed coupling becomes parity even. This is the [axial derivative coupling and parity](../../../relativistic-quantum-field.md#axial-derivative-coupling-and-parity) distinction; parity invariance must not be silently assumed from proper Lorentz invariance.

In four dimensions, $[\phi]=1$, $[\psi]=3/2$ and $[\partial_\mu]=1$. The three operators have [mass dimensions](../../../perturbative-quantum-field-theory.md#mass-dimension) $4,5,6$, respectively. Thus the latter two require dimensionful couplings and are not power-counting renormalizable interactions, but this does not invalidate their Lorentz invariance or their use in an [effective field theory](../../../quantum-field-theory.md#effective-field-theory).

## 2

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For $\mathcal L(A_\nu,\partial_\mu A_\nu)$ define $\Pi^{\mu\nu}=\partial\mathcal L/\partial(\partial_\mu A_\nu)$. A fixed-coordinate infinitesimal field variation $\delta A_\nu=\alpha\Delta_\nu$ satisfying $\delta\mathcal L=\alpha\partial_\mu K^\mu$ gives the [Noether current](../../../quantum-field-theory.md#noether-current)

$$
\boxed{J^\mu=\Pi^{\mu\nu}\Delta_\nu-K^\mu,\qquad
\partial_\mu J^\mu=0\quad\text{on shell}.}
$$

Indeed, the first variation is

$$
\frac{\delta\mathcal L}{\alpha}
=\left(\mathcal L_{A_\nu}-\partial_\mu\Pi^{\mu\nu}\right)\Delta_\nu
+\partial_\mu(\Pi^{\mu\nu}\Delta_\nu);
$$

subtract the divergence of $K$ and use the [Euler-Lagrange field equations](../../../quantum-field-theory.md#euler-lagrange-field-equation). The components of the [Lorentz four-vector](../../../special-relativity.md#four-vector) are simply the field labels in this formula. For a transformation moving the coordinates, use its induced fixed-coordinate variation; this includes translations and [Lorentz transformations](../../../special-relativity.md#lorentz-transformation). The spatial integral of $J^0$ is conserved when the spatial current has vanishing boundary flux.

With signature $(+,-,-,-)$, a [gauge transformation](../../../electromagnetism.md#gauge-transformation) is $A_\mu\mapsto A_\mu+\partial_\mu\chi$. The [electromagnetic field tensor](../../../electromagnetism.md#electromagnetic-field-tensor)

$$
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu
$$

is unchanged, since mixed derivatives of $\chi$ commute. Thus $\mathcal L=-F_{\mu\nu}F^{\mu\nu}/4$ is gauge invariant. Write $A_\mu=(\Phi,-\mathbf A)$, so $F_{0i}=E_i$ and $F_{ij}=-\epsilon_{ijk}B_k$. Then

$$
F_{\mu\nu}F^{\mu\nu}=2(\mathbf B^2-\mathbf E^2),
\qquad
\mathcal L=\frac12(\mathbf E^2-\mathbf B^2).
$$

The overall minus sign produces a positive electric kinetic term and a positive physical [Hamiltonian](../../../classical-mechanics.md#hamiltonian). Reversing it reverses the sign of the physical [energy](../../../classical-mechanics.md#energy) and gives the wrong positive-energy theory; the issue is the indefinite spacetime metric, not negative magnetic [energy](../../../classical-mechanics.md#energy).

For $\Delta_\nu=\partial_0A_\nu$, direct differentiation gives $\delta\mathcal L=\alpha\partial_0\mathcal L=\alpha\partial_\mu(\delta^\mu_0\mathcal L)$. Since

$$
\Pi^{\mu\nu}=-F^{\mu\nu},
$$

the [canonical energy-momentum tensor](../../../quantum-field-theory.md#canonical-stress-energy-tensor) gives the conserved [energy](../../../classical-mechanics.md#energy) current

$$
J^\mu_{\rm can}=-F^{\mu\nu}\partial_0A_\nu-\delta^\mu_0\mathcal L.
$$

Its time component is

$$
J^0_{\rm can}
=\frac12(\mathbf E^2+\mathbf B^2)+\mathbf E\cdot\nabla\Phi,
$$

because $\partial_0 A_i=E_i+\partial_i\Phi$. Thus Noether's conserved canonical [energy](../../../classical-mechanics.md#energy) is $\int J^0_{\rm can}\,d^3x$. In pure, source-free electromagnetism the field equation gives $\nabla\cdot\mathbf E=0$, and

$$
\int\mathbf E\cdot\nabla\Phi\,d^3x
=\int_{\partial V}\Phi\,\mathbf E\cdot d\mathbf S.
$$

For sufficiently decaying fields, or boundary conditions removing this surface term,

$$
\boxed{H=\frac12\int d^3x\,(\mathbf E^2+\mathbf B^2).}
$$

The canonical density is not locally gauge invariant, even though the total [energy](../../../classical-mechanics.md#energy) with these conditions is.

Now use the [gauge-compensated time translation in electromagnetism](../../../electromagnetism.md#gauge-compensated-time-translation-in-electromagnetism),

$$
\Delta_\nu=\partial_0A_\nu-\partial_\nu A_0=F_{0\nu}.
$$

The extra term is a [gauge transformation](../../../electromagnetism.md#gauge-transformation) with the field-dependent parameter $\chi=-\alpha A_0$. It changes no field strength; therefore the combined variation still has $\delta F_{\mu\nu}=\alpha\partial_0F_{\mu\nu}$ and the same $K^\mu=\delta^\mu_0\mathcal L$. The new current is

$$
J^\mu_{\rm inv}=-F^{\mu\nu}F_{0\nu}-\delta^\mu_0\mathcal L.
$$

It is expressed entirely in gauge-invariant field strengths. In particular

$$
\boxed{J^0_{\rm inv}=\frac12(\mathbf E^2+\mathbf B^2),\qquad
\mathbf J_{\rm inv}=\mathbf E\times\mathbf B.}
$$

This is the [energy](../../../classical-mechanics.md#energy) column of the [electromagnetic stress-energy tensor](../../../electromagnetism.md#electromagnetic-stress-energy-tensor)

$$
T^{\mu\nu}=-F^{\mu\rho}F^\nu{}_\rho
+\frac14g^{\mu\nu}F_{\rho\sigma}F^{\rho\sigma}
$$

in the chosen mostly-minus convention. Its conservation is the [energy](../../../classical-mechanics.md#energy) continuity equation.

The currents differ by

$$
J^\mu_{\rm inv}-J^\mu_{\rm can}
=F^{\mu\nu}\partial_\nu A_0
=\partial_\nu(A_0F^{\mu\nu})
$$

on the source-free field equations. The final expression is an antisymmetric superpotential divergence, so it changes the integrated charge only by a boundary term. **The compensating [gauge transformation](../../../electromagnetism.md#gauge-transformation) improves the local [energy](../../../classical-mechanics.md#energy) density without changing the physical conserved [energy](../../../classical-mechanics.md#energy) under the stated boundary conditions.**

## 3

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use signature $(+,-,-,-)$ and the free [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) $(i\gamma^\mu\partial_\mu-m)\psi=0$. For positive $p^0=E_{\mathbf p}=\sqrt{\mathbf p^2+m^2}$, substitution of the two frequency signs gives

$$
\psi=u_s(p)e^{-ip\cdot x}:\quad(\not p-m)u_s(p)=0,
\qquad
\psi=v_s(p)e^{ip\cdot x}:\quad(\not p+m)v_s(p)=0.
$$

Multiplying by the opposite factor shows $p^2=m^2$. Each equation has two independent solutions for a massive field.

In the [Dirac basis](../../../algebra.md#dirac-representation-of-the-gamma-matrices), $\gamma^0=\operatorname{diag}(I,-I)$ and $\gamma^i=\begin{pmatrix}0&\sigma_i\\-\sigma_i&0\end{pmatrix}$. For orthonormal two-component [spin](../../../quantum-mechanics.md#spin) labels $\xi_s,\eta_s$, convenient solutions are

$$
\boxed{u_s(p)=\sqrt{E_{\mathbf p}+m}
\begin{pmatrix}\xi_s\\
\dfrac{\boldsymbol\sigma\cdot\mathbf p}{E_{\mathbf p}+m}\xi_s
\end{pmatrix},\qquad
v_s(p)=\sqrt{E_{\mathbf p}+m}
\begin{pmatrix}
\dfrac{\boldsymbol\sigma\cdot\mathbf p}{E_{\mathbf p}+m}\eta_s\\
\eta_s
\end{pmatrix}.}
$$

The two-block equations verify these expressions using $(\boldsymbol\sigma\cdot\mathbf p)^2=\mathbf p^2I$. At rest the positive-frequency solutions have only upper components and the negative-frequency solutions only lower components. Their normalizations are $u_s^\dagger u_r=v_s^\dagger v_r=2E_{\mathbf p}\delta_{sr}$ and $\bar u_su_r=2m\delta_{sr}$, $\bar v_sv_r=-2m\delta_{sr}$. Their completeness relations are

$$
\sum_su_s(p)\bar u_s(p)=\not p+m,\qquad
\sum_sv_s(p)\bar v_s(p)=\not p-m.
$$

The field expansion combines [fermionic annihilation operators](../../../relativistic-quantum-field.md#fermionic-annihilation-operator) multiplying the positive-frequency waves with [antiparticle](../../../relativistic-quantum-field.md#antiparticle) [fermionic creation operators](../../../relativistic-quantum-field.md#fermionic-creation-operator) multiplying the negative-frequency waves. The latter frequency sign is not the [energy](../../../classical-mechanics.md#energy) of a physical negative-energy [antiparticle](../../../relativistic-quantum-field.md#antiparticle) state.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For the specified $1/\sqrt{2E_{\mathbf p}}$ mode normalization, the [canonical anticommutation relations](../../../quantum-mechanics.md#canonical-anticommutation-relations) are

$$
\boxed{\{a_{\mathbf p}^{s},a_{\mathbf q}^{r\dagger}\}
=\{b_{\mathbf p}^{s},b_{\mathbf q}^{r\dagger}\}
=(2\pi)^3\delta^{sr}\delta^3(\mathbf p-\mathbf q),}
$$

and every other [anticommutator](../../../vector-space.md#anticommutator) of the $a,b$ operators vanishes. For the [Dirac field](../../../relativistic-quantum-field.md#dirac-field), they imply the [Equal-time canonical anticommutator of a Dirac field](../../../quantum-mechanics.md#equal-time-canonical-anticommutator-of-a-dirac-field)

$$
\{\psi_\alpha(t,\mathbf x),\psi_\beta^\dagger(t,\mathbf y)\}
=\delta_{\alpha\beta}\delta^3(\mathbf x-\mathbf y),\qquad
\{\psi_\alpha(t,\mathbf x),\psi_\beta(t,\mathbf y)\}=0.
$$

To check the normalization, the two sectors contribute $u(\mathbf p)u^\dagger(\mathbf p)$ and $v(\mathbf p)v^\dagger(\mathbf p)$ with opposite spatial Fourier signs. Reverse $\mathbf p$ in the second contribution. The completeness relations then give

$$
\sum_s\left[u_s(\mathbf p)u_s^\dagger(\mathbf p)
+v_s(-\mathbf p)v_s^\dagger(-\mathbf p)\right]
=\left[(\not p+m)+(\not{\tilde p}-m)\right]\gamma^0
=2E_{\mathbf p}I,
$$

where $\tilde p=(E_{\mathbf p},-\mathbf p)$. This cancels the mode denominator and leaves the Fourier representation of the delta function. Same-momentum $u^\dagger v$ orthogonality must not be used in place of this reversed-momentum identity.

For arbitrary spacetime points,

$$
\{\psi_\alpha(x),\bar\psi_\beta(y)\}
=(i\not\partial_x+m)_{\alpha\beta}\Delta(x-y),
\qquad
\Delta(z)=\int\frac{d^3p}{(2\pi)^3\,2E_{\mathbf p}}
\left(e^{-ip\cdot z}-e^{ip\cdot z}\right).
$$

For spacelike $z$, choose a Lorentz frame with $z^0=0$; reversing spatial [momentum](../../../classical-mechanics.md#momentum) shows $\Delta(z)=0$. Its derivatives vanish there as well, so the field [anticommutators](../../../vector-space.md#anticommutator) vanish at spacelike separation. This is fermionic [microcausality](../../../relativistic-quantum-field.md#microcausality). The anticommutation rules make the occupation of each normalized mode zero or one, implementing the [Pauli exclusion principle](../../../quantum-mechanics.md#pauli-exclusion-principle), and make the [normal-ordered](../../../perturbative-quantum-field-theory.md#normal-ordering) free [Hamiltonian](../../../classical-mechanics.md#hamiltonian) positive for both particle sectors.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

With a vacuum annihilated by all $a_{\mathbf p}^s,b_{\mathbf p}^s$, define the [particle and antiparticle occupation operators of a Dirac field](../../../relativistic-quantum-field.md#particle-and-antiparticle-occupation-operators-of-a-dirac-field)

$$
N_e=\sum_s\int\frac{d^3p}{(2\pi)^3}a_{\mathbf p}^{s\dagger}a_{\mathbf p}^s,\qquad
N_{\bar e}=\sum_s\int\frac{d^3p}{(2\pi)^3}b_{\mathbf p}^{s\dagger}b_{\mathbf p}^s.
$$

Each counts its corresponding occupied modes. The total positive particle count is

$$
\boxed{N_{\rm total}=N_e+N_{\bar e}.}
$$

Commuting it through either creation operator gives $[N_{\rm total},a^\dagger]=a^\dagger$ and $[N_{\rm total},b^\dagger]=b^\dagger$, so both kinds of one-particle states have eigenvalue one. In a normalized discrete mode, $(a^\dagger a)^2=a^\dagger a$ by the anticommutation relations, so its occupation eigenvalues are $0,1$.

For a [Dirac field](../../../relativistic-quantum-field.md#dirac-field) there is also a distinct conserved signed fermion number. Inserting the mode expansion into the [normal-ordered](../../../perturbative-quantum-field-theory.md#normal-ordering) local density gives

$$
\boxed{Q_D=\int d^3x:\psi^\dagger\psi:
=N_e-N_{\bar e}.}
$$

Spatial integration makes the same-sector momenta equal. The cross terms vanish by $u^\dagger(\mathbf p)v(-\mathbf p)=0$; [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) of $bb^\dagger$ supplies the minus sign for the [antiparticles](../../../relativistic-quantum-field.md#antiparticle). Thus the density integral is not the total positive particle count. It generates the global phase symmetry, and for [Electron](../../../physics.md#electron) charge $-e$ the electric charge is $Q_{\rm em}=-eQ_D$.

The free [normal-ordered](../../../perturbative-quantum-field-theory.md#normal-ordering) [Hamiltonian](../../../classical-mechanics.md#hamiltonian) is

$$
H=\sum_s\int\frac{d^3p}{(2\pi)^3}E_{\mathbf p}
\left(a_{\mathbf p}^{s\dagger}a_{\mathbf p}^s+
b_{\mathbf p}^{s\dagger}b_{\mathbf p}^s\right),
$$

so $N_e,N_{\bar e},N_{\rm total}$ and $Q_D$ are conserved in the free theory. In an interacting theory, pair creation can change the total count while preserving the signed charge. This distinguishes a positive occupation [number operator](../../../quantum-mechanics.md#number-operator) from the charge behind [Dirac fermion number conservation](../../../relativistic-quantum-field.md#dirac-fermion-number-conservation).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

A [Positron](../../../physics.md#positron) is the [Electron](../../../physics.md#electron)'s [antiparticle](../../../relativistic-quantum-field.md#antiparticle): it has the same [mass](../../../classical-mechanics.md#mass) and [spin](../../../quantum-mechanics.md#spin) one-half, opposite electric charge $+e$, and fermionic statistics. A state $b_{\mathbf p}^{s\dagger}|0\rangle$ has positive [energy](../../../classical-mechanics.md#energy) $E_{\mathbf p}$ and physical [momentum](../../../classical-mechanics.md#momentum) $\mathbf p$, as follows from the [Hamiltonian](../../../classical-mechanics.md#hamiltonian) and [momentum](../../../classical-mechanics.md#momentum) operators

$$
[H,b_{\mathbf p}^{s\dagger}]=E_{\mathbf p}b_{\mathbf p}^{s\dagger},
\qquad
[\mathbf P,b_{\mathbf p}^{s\dagger}]
=\mathbf p\,b_{\mathbf p}^{s\dagger}.
$$

The charge [commutator](../../../lie-algebra.md#commutator) gives $[Q_{\rm em},b^\dagger]=+e\,b^\dagger$.

The term $b^\dagger v(p)e^{ip\cdot x}$ in the field has negative frequency, but it creates this positive-energy [Positron](../../../physics.md#positron). Treating its coefficient as an annihilator of a physical negative-energy [Electron](../../../physics.md#electron) would give an unbounded [energy](../../../classical-mechanics.md#energy) interpretation. Fermionic quantization instead reorders that sector, giving positive [antiparticle](../../../relativistic-quantum-field.md#antiparticle) occupation energies and the opposite signed charge. The historical [Dirac sea](../../../relativistic-quantum-field.md#dirac-sea) describes a [Positron](../../../physics.md#positron) as a hole in filled negative-energy [Electron](../../../physics.md#electron) levels; the field-theory interpretation uses an [antiparticle](../../../relativistic-quantum-field.md#antiparticle) creation operator and [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering), without requiring a literal infinite material sea.

Under [charge conjugation of a Dirac field](../../../quantum-field-theory.md#charge-conjugation-of-a-dirac-field), $\psi^C=C\bar\psi^T$, where $C^{-1}\gamma^\mu C=-(\gamma^\mu)^T$, particle and [antiparticle](../../../relativistic-quantum-field.md#antiparticle) modes interchange. [Electron](../../../physics.md#electron)–[Positron](../../../physics.md#positron) pair creation and annihilation change total particle number while conserving electric charge. **[Positrons](../../../physics.md#positron) are positive-energy [antiparticles](../../../relativistic-quantum-field.md#antiparticle), not physical negative-energy [Electrons](../../../physics.md#electron).**

## 4

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use signature $(+,-,-,-)$ and [Electron](../../../physics.md#electron) charge $q=-e$, with $e>0$. Then $\mathcal L_{\rm int}=-q\bar\psi\gamma^\mu\psi A_\mu=+e\bar\psi\gamma^\mu\psi A_\mu$. Write the process as $e^-(p,s)+\gamma(k,\epsilon)\to e^-(p',s')+\gamma(k',\epsilon')$. Physical external states satisfy

$$
p^2=p'^2=m^2,\qquad k^2=k'^2=0,\qquad
p+k=p'+k',\qquad p^0,p'^0,k^0,k'^0>0,
$$

and the [photon polarization vectors](../../../quantum-mechanics.md#photon-polarization-vector) obey $k\cdot\epsilon=k'\cdot\epsilon'=0$. Choose unit physical polarizations with $\epsilon^*\cdot\epsilon=\epsilon'^*\cdot\epsilon'=-1$; representatives differing by a multiple of the corresponding null [momentum](../../../classical-mechanics.md#momentum) describe the same physical polarization. The external spinors obey $(\not p-m)u(p)=0$, $\bar u(p')(\not p'-m)=0$, with $\bar u_su_r=2m\delta_{sr}$. Outgoing polarization appears complex conjugated, so this formula includes helicity states as well as real linear polarizations.

The needed [QED Feynman rules](../../../perturbative-quantum-field-theory.md#qed-feynman-rules) are a vertex $-iq\gamma^\mu=+ie\gamma^\mu$, an internal [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator) $i(\not q+m)/(q^2-m^2+i0)$, the external spinors, and the incoming/outgoing [photon polarization vectors](../../../quantum-mechanics.md#photon-polarization-vector). There is no internal [photon](../../../quantum-mechanics.md#photon) at this order and no elementary two-photon–Dirac seagull vertex. The two [photon](../../../quantum-mechanics.md#photon) orderings along the [Electron](../../../physics.md#electron) line give internal momenta $q_s=p+k$ and $q_u=p-k'$. Defining the [matrix](../../../vector-space.md#matrix) element by $S_{fi}-\delta_{fi}=i(2\pi)^4\delta^4(p+k-p'-k')\mathcal M$, their sum is

$$
\boxed{\mathcal M^{(2)}=-e^2\bar u(p')
\left[
\not\epsilon'^*\frac{\not p+\not k+m}{(p+k)^2-m^2+i0}\not\epsilon
+\not\epsilon\frac{\not p-\not k'+m}{(p-k')^2-m^2+i0}\not\epsilon'^*
\right]u(p).}
$$

The denominators are $2p\cdot k+i0$ and $-2p\cdot k'+i0$. Both terms are essential; this is the [tree-level Compton amplitude](../../../physics.md#tree-level-compton-amplitude).

<a id="4/image-compton-tree-diagrams-and-the-four-one-loop-classes-before-exchanging-the-external-photons"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-44-compton-diagrams.png)

**[Figure 1](#4/image-compton-tree-diagrams-and-the-four-one-loop-classes-before-exchanging-the-external-photons). Compton tree diagrams and the four one-loop classes before exchanging the external photons**.

To prove the incoming [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity), replace $\epsilon$ by $k$ and write $R(q)=(\not q+m)/(q^2-m^2)$, with the Feynman boundary prescription understood. The physical nonzero-photon kinematics keeps these tree denominators off the [Electron](../../../physics.md#electron) pole. Since

$$
\not k=(\not q_s-m)-(\not p-m),
\qquad
\not k=(\not p'-m)-(\not q_u-m),
$$

the external [Dirac equations](../../../relativistic-quantum-field.md#dirac-equation) imply

$$
R(q_s)\not k\,u(p)=u(p),\qquad
\bar u(p')\not k\,R(q_u)=-\bar u(p').
$$

Therefore the two contracted terms are $\bar u(p')\not\epsilon'^*u(p)$ and its negative, and cancel. By linearity,

$$
\boxed{\mathcal M(\epsilon+\alpha k)=\mathcal M(\epsilon).}
$$

This is the [two-photon fermion Ward identity](../../../perturbative-quantum-field-theory.md#two-photon-fermion-ward-identity). An analogous cancellation holds for the outgoing [photon](../../../quantum-mechanics.md#photon). Gauge-equivalent polarization representatives have the same scattering amplitude, so a longitudinal pure-gauge component is not an extra physical [photon](../../../quantum-mechanics.md#photon) state. Individual diagrams do not generally satisfy this identity; their sum does.

For perturbative order, each elementary [QED](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics) vertex has one [photon](../../../quantum-mechanics.md#photon) leg. If $I_\gamma$ is the number of internal [photon](../../../quantum-mechanics.md#photon) lines and $E_\gamma=2$, the [vertex parity of a QED amplitude](../../../perturbative-quantum-field-theory.md#vertex-parity-of-a-qed-amplitude) gives

$$
V=2I_\gamma+2.
$$

Thus **there is no third-order contribution**. At fourth order, $V=4$ and, counting all three legs per vertex with four external legs, $I=(3V-4)/2=4$. A connected graph has loop number $I-V+1=1$.

The nonzero one-loop classes on the open [Electron](../../../physics.md#electron) line are an internal-electron [self-energy](../../../perturbative-quantum-field-theory.md#self-energy) insertion, a vertex correction at either external-photon vertex, and a virtual [photon](../../../quantum-mechanics.md#photon) spanning both [photon](../../../quantum-mechanics.md#photon) vertices, giving the four-point box class. The first figure sketches each class for one [photon](../../../quantum-mechanics.md#photon) ordering; interchange the two external [photon](../../../quantum-mechanics.md#photon) attachments for its crossed partner. This yields two internal-self-energy graphs, four vertex graphs and two spanning-box graphs. They use the usual [photon](../../../quantum-mechanics.md#photon) propagator, for example $-ig_{\mu\nu}/(\ell^2+i0)$ in [Feynman gauge](../../../relativistic-quantum-field.md#feynman-gauge).

<a id="4/image-external-leg-insertions-fourth-order-counterterms-and-the-odd-photon-loops-that-cancel"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-44-compton-bookkeeping.png)

**[Figure 2](#4/image-external-leg-insertions-fourth-order-counterterms-and-the-odd-photon-loops-that-cancel). External-leg insertions, fourth-order counterterms and the odd-photon loops that cancel**.

For completeness, [one-loop diagram classes for Compton scattering](../../../physics.md#one-loop-diagram-classes-for-compton-scattering) also depend on whether one is drawing an unamputated correlation function or a physical amplitude. [Electron](../../../physics.md#electron) self-energies can be attached to either external [Electron](../../../physics.md#electron) leg, and [photon vacuum polarization](../../../perturbative-quantum-field-theory.md#photon-vacuum-polarization) can be attached to either external [photon](../../../quantum-mechanics.md#photon) leg, for both [photon](../../../quantum-mechanics.md#photon) orders. In an on-shell renormalized [S-matrix](../../../quantum-mechanics.md#s-matrix), these are accounted for by [LSZ reduction](../../../perturbative-quantum-field-theory.md#lsz-reduction-formula) and external-field residues rather than counted again as independent amputated graphs. Photon-leg corrections are not vacuum-polarization insertions on an internal Born [photon](../../../quantum-mechanics.md#photon): there is no such Born line.

At the same fourth order, a renormalized calculation has one [mass](../../../classical-mechanics.md#mass) or electron-field [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) on the internal [Electron](../../../physics.md#electron) line, or one vertex [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) at either Born vertex; the crossed partners are included. Each [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) is a relative order-$e^2$ correction to the order-$e^2$ tree amplitude. External-field normalization must follow the same convention.

A possible closed [Electron](../../../physics.md#electron) loop with three [photon](../../../quantum-mechanics.md#photon) vertices, linked to the external [Electron](../../../physics.md#electron) line by a virtual [photon](../../../quantum-mechanics.md#photon), cancels between its two orientations by [Furry's theorem](../../../quantum-field-theory.md#furry-s-theorem). Transposing the loop and using $C^{-1}\gamma^\mu C=-(\gamma^\mu)^T$ gives an extra sign $(-1)^3$, so its orientation-reversed partner is its negative. A one-photon tadpole likewise vanishes. Disconnected vacuum bubbles are removed by vacuum normalization. **The first genuine radiative corrections are fourth order, with the internal [self-energy](../../../perturbative-quantum-field-theory.md#self-energy), vertex and spanning-box classes and their consistently included [renormalization](../../../perturbative-quantum-field-theory.md#renormalization) terms.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
