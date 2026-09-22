# Paper 62

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper62.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper62.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use units $\hbar=c=1$ and the [Minkowski metric](../../../special-relativity.md#minkowski-metric) $g=\operatorname{diag}(1,-1,-1,-1)$. The [canonical momentum](../../../classical-mechanics.md#canonical-momentum) of the [real scalar field](../../../scalar-field-theory.md#real-scalar-field) is $\pi=\partial\mathcal L/\partial\dot\phi=\dot\phi$. [Canonical quantization](../../../quantum-mechanics.md#canonical-quantization) replaces the classical fields by [operator-valued distributions](../../../quantum-field-theory.md#operator-valued-distribution) and imposes the equal-time [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation)

$$
[\phi(t,\mathbf x),\pi(t,\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y),\qquad [\phi(t,\mathbf x),\phi(t,\mathbf y)]=[\pi(t,\mathbf x),\pi(t,\mathbf y)]=0.
$$

These relations are imposed on an initial slice, with smeared fields understood. In the [Heisenberg picture](../../../quantum-mechanics.md#heisenberg-picture), simultaneous [unitary time evolution](../../../quantum-mechanics.md#unitary-time-evolution) of both operators preserves their [commutators](../../../lie-algebra.md#commutator). Since the momentum is $\dot\phi$, **the requested equal-time commutator is** $[\phi(t,\mathbf x),\dot\phi(t,\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y)$.

The [Legendre transform in mechanics](../../../classical-mechanics.md#legendre-transform-in-mechanics), applied pointwise, gives the [canonical Hamiltonian density of a real scalar field](../../../quantum-field-theory.md#canonical-hamiltonian-density-of-a-real-scalar-field). Thus

$$
\boxed{H=\frac12\int d^3x\,[\pi^2+|\nabla\phi|^2+m^2\phi^2].}
$$

To obtain its dynamics rather than assume them, use the [Heisenberg equation of motion](../../../quantum-mechanics.md#heisenberg-equation-of-motion) $\dot O=i[H,O]$. The momentum-square term gives $[H,\phi]=-i\pi$. The field-square term gives $[H,\pi]=im^2\phi$, while differentiating the [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) in the gradient term and integrating by parts gives $[H,\pi]=-i\nabla^2\phi+im^2\phi$. Consequently

$$
\dot\phi=\pi,\qquad \dot\pi=\nabla^2\phi-m^2\phi,\qquad \boxed{(\Box+m^2)\phi=0.}
$$

Boundary terms vanish for suitably decaying smeared fields. This is the [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) as an operator identity.

A spatial [Fourier transform](../../../analysis.md#fourier-transform) reduces the [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) to $\ddot\phi_{\mathbf p}+E_p^2\phi_{\mathbf p}=0$, where $E_p=\sqrt{\mathbf p^2+m^2}$. Its two frequency branches and the [Hermitian adjoint](../../../hilbert-space.md#adjoint-operator) condition give

$$
\phi(x)=\int d\Pi_p\,[a(p)e^{-ip\cdot x}+a^\dagger(p)e^{ip\cdot x}],\qquad d\Pi_p=\frac{d^3p}{(2\pi)^3 2E_p},\quad p^0=E_p.
$$

The [invariant-normalized scalar mode extraction](../../../quantum-field-theory.md#invariant-normalized-scalar-mode-extraction) can be written particularly simply as

$$
a(p)=\int d^3x\,e^{ip\cdot x}[E_p\phi(x)+i\pi(x)],\qquad a^\dagger(p)=\int d^3x\,e^{-ip\cdot x}[E_p\phi(x)-i\pi(x)].
$$

Substituting the [mode expansion of a free field](../../../quantum-field-theory.md#mode-expansion-of-a-free-field) proves these inversion formulas: the opposite-frequency coefficient is proportional to $E_p-E_q$ and vanishes after spatial [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem). Alternatively they are the corresponding [Klein-Gordon inner products](../../../quantum-field-theory.md#klein-gordon-inner-product). Taking their [commutators](../../../lie-algebra.md#commutator) using the equal-time fields gives $(E_p+E_q)(2\pi)^3\delta^{(3)}(\mathbf p-\mathbf q)$ in the mixed case. In the two equal-type cases the delta function enforces $\mathbf q=-\mathbf p$, multiplying $E_p-E_q=0$. Therefore

$$
\boxed{[a(p),a^\dagger(q)]=(2\pi)^3 2E_p\delta^{(3)}(\mathbf p-\mathbf q),\qquad [a(p),a(q)]=[a^\dagger(p),a^\dagger(q)]=0.}
$$

Conversely these mode [commutators](../../../lie-algebra.md#commutator) reproduce $[\phi,\dot\phi]=i\delta^{(3)}$: the two frequency contributions each supply half the spatial [Dirac delta function](../../../distribution-theory.md#dirac-delta-function).

For the [covariant oscillator Hamiltonian of a real scalar field](../../../scalar-field-theory.md#covariant-oscillator-hamiltonian-of-a-real-scalar-field), insert the [mode expansion of a free field](../../../quantum-field-theory.md#mode-expansion-of-a-free-field) into $H$. Spatial integration sets the two momenta equal in the mixed terms and opposite in the two-creator or two-annihilator terms. The latter have coefficient $-E_p^2+\mathbf p^2+m^2=0$. The mixed terms give

$$
H=\frac12\int d\Pi_p\,E_p[a^\dagger(p)a(p)+a(p)a^\dagger(p)]
=\int d\Pi_p\,E_p a^\dagger(p)a(p)+E_0,
\qquad E_0=\frac12\int d^3p\,E_p\delta^{(3)}(0).
$$

The constant $E_0$ is the divergent [zero-point energy](../../../quantum-mechanics.md#zero-point-energy); a finite box and a momentum cutoff make its meaning explicit. [Normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering) sets the free [vacuum energy](../../../perturbative-quantum-field-theory.md#vacuum-energy) to zero and leaves all [commutators](../../../lie-algebra.md#commutator) unchanged. Directly applying the mode [commutators](../../../lie-algebra.md#commutator) to the mixed expression yields

$$
\boxed{[H,a(p)]=-E_pa(p),\qquad [H,a^\dagger(p)]=E_pa^\dagger(p).}
$$

Choose the [Fock vacuum](../../../quantum-field-theory.md#fock-vacuum) by $a(p)|0\rangle=0$. Each [creation operator](../../../quantum-mechanics.md#creation-operator) adds a [boson](../../../quantum-mechanics.md#boson) of energy $E_p$ and [four-momentum](../../../special-relativity.md#four-momentum) $p$, while each [annihilation operator](../../../quantum-mechanics.md#annihilation-operator) removes one. Products of commuting [creation operators](../../../quantum-mechanics.md#creation-operator) give [bosonic statistics from commuting creation operators](../../../quantum-mechanics.md#bosonic-statistics-from-commuting-creation-operators) and unrestricted [occupation numbers](../../../quantum-field-theory.md#occupation-number). The [real scalar field](../../../scalar-field-theory.md#real-scalar-field) has one spin-zero species, identical to its [antiparticle](../../../relativistic-quantum-field.md#antiparticle). Its [one-particle states](../../../quantum-field-theory.md#one-particle-state) obey $\langle q|p\rangle=(2\pi)^3 2E_p\delta^{(3)}(\mathbf p-\mathbf q)$, precisely the [relativistic normalization of a one-particle state](../../../quantum-field-theory.md#relativistic-normalization-of-a-one-particle-state).

For the [Feynman propagator](../../../quantum-field-theory.md#feynman-propagator), put $z=x-y$ and contract the two fields in the [Fock vacuum](../../../quantum-field-theory.md#fock-vacuum). Only $aa^\dagger$ survives, giving the [Wightman function](../../../quantum-field-theory.md#wightman-function)

$$
W(z)=\langle0|\phi(x)\phi(y)|0\rangle=\int d\Pi_p\,e^{-ip\cdot z}.
$$

The stipulated [time-ordered product](../../../perturbative-quantum-field-theory.md#time-ordered-product) convention is $i\Delta_F(z)=\theta(z^0)W(z)+\theta(-z^0)W(-z)$. In a [contour integral](../../../complex-analysis.md#contour-integral) over $p^0$, the [Feynman i-epsilon prescription](../../../quantum-field-theory.md#feynman-i-epsilon-prescription) places the positive-energy pole just below the real axis and the negative-energy pole just above it. For $z^0>0$ close below, clockwise, obtaining $-i e^{-iE_pz^0}/(2E_p)$; for $z^0<0$ close above, obtaining $-i e^{iE_pz^0}/(2E_p)$. Changing $\mathbf p\mapsto-\mathbf p$ in the second contribution therefore proves

$$
\boxed{\Delta_F(z)=\lim_{\epsilon\downarrow0}\int\frac{d^4p}{(2\pi)^4}\frac{e^{-ip\cdot z}}{p^2-m^2+i\epsilon}.}
$$

Acting with $\Box+m^2$ multiplies the integrand by $-(p^2-m^2)$. The remaining factor tends to $-1$ as a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis), so [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem) gives

$$
\boxed{(\Box+m^2)\Delta_F(z)=-\delta^{(4)}(z).}
$$

The sign also follows from the [derivative jump of a free scalar time-ordered two-point function](../../../quantum-field-theory.md#derivative-jump-of-a-free-scalar-time-ordered-two-point-function): the first time derivative of $i\Delta_F$ jumps by $\langle[\dot\phi,\phi]\rangle=-i\delta^{(3)}$, so that of $\Delta_F$ jumps by $-\delta^{(3)}$.

## 2

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For the [complex scalar field](../../../scalar-field-theory.md#complex-scalar-field), the [canonical momenta](../../../classical-mechanics.md#canonical-momentum) are $\pi=\dot\phi^\dagger$ and $\pi^\dagger=\dot\phi$. Split $H=H_0+H_I$. The [interaction picture](../../../quantum-mechanics.md#interaction-picture) is obtained from the [Schrödinger picture](../../../quantum-mechanics.md#schrodinger-picture) by $|\Psi_I(t)\rangle=e^{iH_0t}|\Psi_S(t)\rangle$ and $O_I(t)=e^{iH_0t}O_Se^{-iH_0t}$, choosing a common time origin. The fields therefore obey the free [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation), while the states evolve through $H_I(t)$. The [canonical quantization of a complex scalar field](../../../scalar-field-theory.md#canonical-quantization-of-a-complex-scalar-field) gives

$$
\phi_I(x)=\int d\Pi_p\,[a(p)e^{-ip\cdot x}+b^\dagger(p)e^{ip\cdot x}],\qquad d\Pi_p=\frac{d^3p}{(2\pi)^3 2E_p}.
$$

The adjoint expansion contains $a^\dagger$ and $b$. Particle and [antiparticle](../../../relativistic-quantum-field.md#antiparticle) modes are independent; their nonzero [commutators](../../../lie-algebra.md#commutator) are

$$
\boxed{[a(p),a^\dagger(q)]=[b(p),b^\dagger(q)]=(2\pi)^3 2E_p\delta^{(3)}(\mathbf p-\mathbf q).}
$$

All cross-species [commutators](../../../lie-algebra.md#commutator), and all pairs of [creation operators](../../../quantum-mechanics.md#creation-operator) or of [annihilation operators](../../../quantum-mechanics.md#annihilation-operator), vanish. These formulas reproduce $[\phi(\mathbf x),\pi(\mathbf y)]=[\phi^\dagger(\mathbf x),\pi^\dagger(\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y)$ and the remaining vanishing equal-time [commutators](../../../lie-algebra.md#commutator).

There are no derivative interactions, so the [interaction Hamiltonian](../../../quantum-field-theory.md#interaction-hamiltonian) is $H_I(t)=-\int d^3x\,\mathcal L_I(x)$. Differentiating the [interaction picture](../../../quantum-mechanics.md#interaction-picture) state gives $i\partial_t|\Psi_I\rangle=H_I(t)|\Psi_I\rangle$. Its [time-evolution operator](../../../quantum-mechanics.md#time-evolution-operator) satisfies

$$
U(t,t_0)=I-i\int_{t_0}^t dt_1\,H_I(t_1)U(t_1,t_0).
$$

Iteration gives ordered integration regions $t_1>\cdots>t_n$. Each is $1/n!$ of the full region with a [time-ordered product](../../../perturbative-quantum-field-theory.md#time-ordered-product), yielding the [Dyson series](../../../perturbative-quantum-field-theory.md#dyson-series)

$$
U(t,t_0)=\sum_{n=0}^\infty\frac{(-i)^n}{n!}\int_{t_0}^t dt_1\cdots dt_n\,T[H_I(t_1)\cdots H_I(t_n)].
$$

With the usual asymptotic scattering prescription, taking $t_0\to-\infty$ and $t\to+\infty$ proves

$$
\boxed{S=T\exp\!\left(i\int d^4x\,\mathcal L_I(x)\right).}
$$

[Time ordering](../../../perturbative-quantum-field-theory.md#time-ordering) is essential because different interaction Hamiltonians need not commute.

At first order, use the connected tree [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude), equivalently the [normal-ordered](../../../perturbative-quantum-field-theory.md#normal-ordering) quartic vertex with the vacuum and one-particle mass contributions removed. This qualification matters if the local product is interpreted literally without [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering): single-vertex [tadpole diagrams](../../../perturbative-quantum-field-theory.md#tadpole-diagram) and [vacuum diagrams](../../../perturbative-quantum-field-theory.md#vacuum-feynman-diagram) are not the requested connected two-particle amplitude. The [complex scalar quartic contact vertex](../../../scalar-field-theory.md#complex-scalar-quartic-contact-vertex) is obtained from

$$
S-I=-\frac{i\lambda}{4}\int d^4x\,:\!\phi^{\dagger 2}(x)\phi^2(x)\!:+O(\lambda^2).
$$

In a fully connected matrix element, an incoming particle and outgoing antiparticle attach to the two $\phi$ factors; an outgoing particle and incoming antiparticle attach to the two $\phi^\dagger$ factors. Each pair has two assignments, giving $2!2!=4$. The external [relativistic normalization of a one-particle state](../../../quantum-field-theory.md#relativistic-normalization-of-a-one-particle-state) cancels each mode measure: for example $[\phi(x),a^\dagger(p_1)]=e^{-ip_1x}$ and $[b(q_2),\phi(x)]=e^{iq_2x}$. Consequently the connected integrand is $4e^{-i(p_1+q_1-p_2-q_2)\cdot x}$, and

$$
\langle p_2q_2|(S-I)|p_1q_1\rangle_{\rm conn}
=-i\lambda(2\pi)^4\delta^{(4)}(p_1+q_1-p_2-q_2)+O(\lambda^2).
$$

Thus **the invariant connected amplitude is**

$$
\boxed{\mathcal T=-\lambda+O(\lambda^2).}
$$

The [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) expresses [four-momentum conservation](../../../special-relativity.md#four-momentum-conservation).

For the identity contribution, commute $a(p_2)$ through $a^\dagger(p_1)$ and independently $b(q_2)$ through $b^\dagger(q_1)$; all terms leaving a [creation operator](../../../quantum-mechanics.md#creation-operator) against the left [Fock vacuum](../../../quantum-field-theory.md#fock-vacuum) or an [annihilation operator](../../../quantum-mechanics.md#annihilation-operator) against the right [Fock vacuum](../../../quantum-field-theory.md#fock-vacuum) vanish. Hence

$$
\boxed{\langle p_2q_2|I|p_1q_1\rangle=(2\pi)^6(2E_{p_1})(2E_{q_1})\delta^{(3)}(\mathbf p_2-\mathbf p_1)\delta^{(3)}(\mathbf q_2-\mathbf q_1).}
$$

There is no exchange term between the two distinct particle and [antiparticle](../../../relativistic-quantum-field.md#antiparticle) species.

## 3

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the [Minkowski metric](../../../special-relativity.md#minkowski-metric) $g^{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ and [Feynman slash notation](../../../algebra.md#feynman-slash-notation) $\not p=\gamma^\mu p_\mu$. The [Pauli matrices](../../../algebra.md#pauli-matrices) satisfy $\sigma_j\sigma_k+\sigma_k\sigma_j=2\delta_{jk}I_2$. In the [Dirac representation of the gamma matrices](../../../algebra.md#dirac-representation-of-the-gamma-matrices), direct block multiplication gives

$$
(\gamma^0)^2=I_4,\qquad \gamma^0\gamma^j=\begin{pmatrix}0&\sigma_j\\\sigma_j&0\end{pmatrix}=-\gamma^j\gamma^0,
$$

and

$$
\gamma^j\gamma^k=\begin{pmatrix}-\sigma_j\sigma_k&0\\0&-\sigma_j\sigma_k\end{pmatrix}.
$$

Thus the spatial [anticommutators](../../../vector-space.md#anticommutator) are $-2\delta_{jk}I_4$, proving **the Clifford relations**

$$
\boxed{\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu}I_4.}
$$

Since partial derivatives commute, their symmetric product selects the symmetric part of the [gamma matrices](../../../algebra.md#gamma-matrices). Multiplying the [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) by $i\gamma^\mu\partial_\mu+m$ gives

$$
(i\not\partial+m)(i\not\partial-m)\psi
=(-\gamma^\mu\gamma^\nu\partial_\mu\partial_\nu-m^2)\psi
=-(\Box+m^2)\psi=0.
$$

Hence **every spinor component satisfies the Klein-Gordon equation** with the same mass.

For [parity](../../../quantum-mechanics.md#parity), let $x_P=(t,-\mathbf x)$ and $\psi_P(x)=\gamma^0\psi(x_P)$. The chain rule gives $\partial_0\psi(x_P)=(\partial_0\psi)(x_P)$ and $\partial_j\psi(x_P)=-(\partial_j\psi)(x_P)$. Combining these signs with $\gamma^j\gamma^0=-\gamma^0\gamma^j$ proves

$$
(i\not\partial-m)\psi_P(x)
=\gamma^0[(i\not\partial-m)\psi](x_P)=0.
$$

This establishes [parity symmetry in quantum field theory](../../../quantum-field-theory.md#parity-symmetry-in-quantum-field-theory) for the free [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation), rather than merely asserting its covariance.

A positive-energy [plane wave](../../../quantum-mechanics.md#plane-wave) $\psi=u(p)e^{-ip\cdot x}$ solves $(\not p-m)u=0$. Write $u=(\chi,\eta)^T$. The two block equations are

$$
(E_p-m)\chi-(\boldsymbol\sigma\cdot\mathbf p)\eta=0,\qquad
(\boldsymbol\sigma\cdot\mathbf p)\chi-(E_p+m)\eta=0.
$$

The second gives $\eta=(\boldsymbol\sigma\cdot\mathbf p)\chi/(E_p+m)$. In the first, $(\boldsymbol\sigma\cdot\mathbf p)^2=\mathbf p^2 I_2$ and $E_p^2-\mathbf p^2=m^2$ make the remaining coefficient zero. There are two independent two-component choices $\chi_s$, so

$$
\boxed{u_s(p)=\begin{pmatrix}\chi_s\\(\boldsymbol\sigma\cdot\mathbf p)\chi_s/(E_p+m)\end{pmatrix},\qquad \psi_{p,s}(x)=u_s(p)e^{-ip\cdot x}.}
$$

For a massive [Dirac spinor](../../../relativistic-quantum-field.md#dirac-spinor), choose $\chi_s$ as the two rest-frame [spin](../../../quantum-mechanics.md#spin) states along a fixed axis, for example $\sigma_3\chi_s=\pm\chi_s$. The label $s$ distinguishes these canonical [spin](../../../quantum-mechanics.md#spin) states after boosting; it is not automatically a [helicity](../../../special-relativity.md#helicity) label.

Now $p\cdot x_P=p_P\cdot x$ and $\gamma^0u_s(p)=u_s(p_P)$ for the same fixed $\chi_s$. Therefore

$$
\boxed{\psi_{p,s}(x)\longmapsto\psi_{p_P,s}(x).}
$$

The [parity action on canonical massive spin states](../../../quantum-field-theory.md#parity-action-on-canonical-massive-spin-states) leaves the canonical [spin](../../../quantum-mechanics.md#spin) label unchanged while reversing the [momentum](../../../classical-mechanics.md#momentum). [Spin](../../../quantum-mechanics.md#spin) is an axial vector under [parity](../../../quantum-mechanics.md#parity); its orientation is unchanged. Consequently [helicity](../../../special-relativity.md#helicity), the projection of [spin](../../../quantum-mechanics.md#spin) along [momentum](../../../classical-mechanics.md#momentum), reverses. If $s$ had instead been chosen to denote [helicity](../../../special-relativity.md#helicity), the transformed label would have the opposite sign.

The [Dirac adjoint](../../../relativistic-quantum-field.md#dirac-adjoint) is $\bar\psi=\psi^\dagger\gamma^0$, with $\gamma^{0\dagger}=\gamma^0$. Thus

$$
\bar\psi_P(x)=[\gamma^0\psi(x_P)]^\dagger\gamma^0=\psi^\dagger(x_P)=\bar\psi(x_P)\gamma^0.
$$

The [chirality matrix](../../../algebra.md#chirality-matrix) has $\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3=\begin{pmatrix}0&I_2\\I_2&0\end{pmatrix}$ in this representation, so $(\gamma^5)^2=I_4$ and it anticommutes with every $\gamma^\mu$. In particular $\gamma^0\gamma^5\gamma^0=-\gamma^5$. The [parity transformation of a Dirac bilinear](../../../quantum-field-theory.md#parity-transformation-of-a-dirac-bilinear) therefore yields

$$
\boxed{\bar\psi_P(x)\psi_P(x)=\bar\psi(x_P)\psi(x_P),\qquad
\bar\psi_P(x)\gamma^5\psi_P(x)=-\bar\psi(x_P)\gamma^5\psi(x_P).}
$$

The first bilinear is a scalar under [parity](../../../quantum-mechanics.md#parity), whereas the second is a [pseudoscalar](../../../quantum-mechanics.md#pseudoscalar).

For the requested [gamma matrix trace identities](../../../algebra.md#gamma-matrix-trace-identities), use the [cyclic property of the trace](../../../linear-algebra.md#cyclic-property-of-the-trace). Conjugation of a product of $n$ [gamma matrices](../../../algebra.md#gamma-matrices) by $\gamma^5$ multiplies it by $(-1)^n$, but leaves its [trace](../../../linear-algebra.md#matrix-trace) unchanged. All odd products therefore have zero [trace](../../../linear-algebra.md#matrix-trace). Taking the [trace](../../../linear-algebra.md#matrix-trace) of the [Clifford algebra](../../../algebra.md#clifford-algebra) relation and using $\operatorname{Tr}I_4=4$ gives $\operatorname{Tr}(\gamma^\alpha\gamma^\beta)=4g^{\alpha\beta}$. For four factors, move the first [gamma matrix](../../../algebra.md#gamma-matrices) successively past the next three using the [anticommutators](../../../vector-space.md#anticommutator). If $A=\operatorname{Tr}(\gamma^\alpha\gamma^\beta\gamma^\rho\gamma^\delta)$, this gives

$$
A=2g^{\alpha\beta}\operatorname{Tr}(\gamma^\rho\gamma^\delta)
-2g^{\alpha\rho}\operatorname{Tr}(\gamma^\beta\gamma^\delta)
+2g^{\alpha\delta}\operatorname{Tr}(\gamma^\beta\gamma^\rho)-A.
$$

Thus $A=4(g^{\alpha\beta}g^{\rho\delta}-g^{\alpha\rho}g^{\beta\delta}+g^{\alpha\delta}g^{\beta\rho})$. Contracting with the relevant [four-vectors](../../../special-relativity.md#four-vector) proves all four answers:

$$
\boxed{\begin{aligned}
\operatorname{Tr}(\not p)&=0,\\
\operatorname{Tr}(\not p\not q)&=4p\cdot q,\\
\operatorname{Tr}(\not p\not q\not k)&=0,\\
\operatorname{Tr}(\not p\gamma^\mu\not q\gamma^\nu)&=4[p^\mu q^\nu+p^\nu q^\mu-(p\cdot q)g^{\mu\nu}].
\end{aligned}}
$$

## 4

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The original PDF contains three algebraic misprints in this question. The second internal [four-momentum](../../../special-relativity.md#four-momentum) must consistently be $r'_k$, since it is defined by $r'_k=q_k-p'=r_i-q_j$. Its [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator) denominator is $(r'_k)^2-m^2$, including after contracting the first photon; the printed plus sign is incorrect. Finally, the middle-photon contraction must retain the mass term in both remaining [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator) numerators. The following calculation keeps the electron mass and proves the corrected identities.

Write $r=p-q_i$, $R=q_k-p'=r-q_j$ and introduce

$$
D(l)=\not l-m,\qquad F(l)=D(l)^{-1}=\frac{\not l+m}{l^2-m^2}.
$$

Here $F$ is the matrix part of the [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator), with the overall factors of $i$ kept in the common amplitude convention. The [Clifford algebra](../../../algebra.md#clifford-algebra) proves $D(l)F(l)=F(l)D(l)=I$. At tree level the intermediate lines here are off their [mass shell](../../../special-relativity.md#mass-shell), so this inverse can be used directly; the usual [Feynman i-epsilon prescription](../../../quantum-field-theory.md#feynman-i-epsilon-prescription) defines its continuation at poles. With $C=(ie)^3$, the consistently routed tensor is

$$
T_{ijk}^{\mu\nu\sigma}=C\bar v(p')\gamma^\sigma F(R)\gamma^\nu F(r)\gamma^\mu u(p).
$$

The external [Dirac equations](../../../relativistic-quantum-field.md#dirac-equation) are $(\not p-m)u(p)=0$ and $\bar v(p')(\not p'+m)=0$.

For the photon at the electron end, $\not q_i=\not p-\not r$ and hence $\not q_i u=-D(r)u$. Multiplication by $F(r)$ removes that internal line, giving

$$
\boxed{T_{ijk}^{\mu\nu\sigma}q_{i\mu}=-C\bar v(p')\gamma^\sigma F(R)\gamma^\nu u(p).}
$$

For the middle photon, $\not q_j=D(r)-D(R)$. Associativity, without any commuting of [gamma matrices](../../../algebra.md#gamma-matrices), gives

$$
F(R)\not q_j F(r)=F(R)D(r)F(r)-F(R)D(R)F(r)=F(R)-F(r).
$$

Therefore

$$
\boxed{T_{ijk}^{\mu\nu\sigma}q_{j\nu}=C\bar v(p')\gamma^\sigma\left[\frac{\not R+m}{R^2-m^2}-\frac{\not r+m}{r^2-m^2}\right]\gamma^\mu u(p).}
$$

Omitting the two mass numerators changes this expression by

$$
Cm\left[\frac1{R^2-m^2}-\frac1{r^2-m^2}\right]\bar v(p')\gamma^\sigma\gamma^\mu u(p),
$$

which need not vanish. For a concrete counterexample take $m=1$, $p=(2,0,0,\sqrt3)$, $p'= (2,0,0,-\sqrt3)$ and outgoing [photon](../../../quantum-mechanics.md#photon) momenta $q_1=(1,1,0,0)$, $q_2=(6/5,2/5,4\sqrt2/5,0)$, $q_3=(9/5,-7/5,-4\sqrt2/5,0)$. All external momenta are [on shell](../../../quantum-field-theory.md#on-shell) and conserve [four-momentum](../../../special-relativity.md#four-momentum). Choose the upper two-spinor $(1,0)^T$ for $u$ and the lower two-spinor $(1,0)^T$ for $v$, with the other blocks fixed by the [Dirac equations](../../../relativistic-quantum-field.md#dirac-equation). For $(i,j,k)=(1,2,3)$ and $(\mu,\sigma)=(0,3)$, the correct middle contraction divided by $C$ is $1/3$, whereas the expression with the mass numerators omitted is $5/27$. Thus the printed middle identity is not valid for a massive [Electron](../../../physics.md#electron).

At the positron end, $q_k=R+p'$. The adjoint [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) gives $\bar v\not q_k=\bar v(\not R-m)=\bar vD(R)$, so the remaining requested contraction is

$$
\boxed{T_{ijk}^{\mu\nu\sigma}q_{k\sigma}=C\bar v(p')\gamma^\nu F(r)\gamma^\mu u(p).}
$$

The opposite signs at the two ends are precisely what makes the [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity) work.

There is one [Feynman diagram](../../../perturbative-quantum-field-theory.md#feynman-diagram) for each order in which the three outgoing [photons](../../../quantum-mechanics.md#photon) attach to the electron line. Their orders, encountered from the incoming [Electron](../../../physics.md#electron) to the incoming [Positron](../../../physics.md#positron), are $(1,2,3)$, $(1,3,2)$, $(2,1,3)$, $(2,3,1)$, $(3,1,2)$ and $(3,2,1)$.

<a id="4/image-the-six-tree-diagrams-for-electron-positron-annihilation-into-three-photons-ordered-along-fermion-flow"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-62-three-photon-diagrams.png)

**[Figure 1](#4/image-the-six-tree-diagrams-for-electron-positron-annihilation-into-three-photons-ordered-along-fermion-flow). The six tree diagrams for electron-positron annihilation into three photons, ordered along fermion flow**.

The straight-line arrows indicate [fermion flow](../../../perturbative-quantum-field-theory.md#fermion-flow); the incoming [Positron](../../../physics.md#positron) momentum is opposite to its line's [fermion flow](../../../perturbative-quantum-field-theory.md#fermion-flow). Each wavy branch is an outgoing [photon](../../../quantum-mechanics.md#photon), and the order shown in a panel fixes the two internal [Dirac propagators](../../../quantum-field-theory.md#dirac-propagator).

To prove the full [three-photon fermion Ward identity](../../../perturbative-quantum-field-theory.md#three-photon-fermion-ward-identity), replace the [photon polarization vector](../../../quantum-mechanics.md#photon-polarization-vector) of one fixed photon $\ell$ by its [four-momentum](../../../special-relativity.md#four-momentum) $q_\ell$. Fix the order $(a,b)$ of the other two [photons](../../../quantum-mechanics.md#photon) and write $\Gamma_a=\not\epsilon_a$, $\Gamma_b=\not\epsilon_b$. There are exactly three positions for photon $\ell$ relative to that order. By the three contractions just derived, their contributions, divided by $C$, are

$$
\begin{aligned}
(\ell,a,b):\quad&-\bar v\Gamma_b F(q_b-p')\Gamma_a u,\\
(a,\ell,b):\quad&\bar v\Gamma_b[F(q_b-p')-F(p-q_a)]\Gamma_a u,\\
(a,b,\ell):\quad&+\bar v\Gamma_b F(p-q_a)\Gamma_a u.
\end{aligned}
$$

[Four-momentum conservation](../../../special-relativity.md#four-momentum-conservation) $p+p'=q_\ell+q_a+q_b$ identifies the shared internal momenta in these expressions. The three terms cancel exactly. Repeating for the other order $(b,a)$ covers all six [Feynman diagrams](../../../perturbative-quantum-field-theory.md#feynman-diagram), and proves

$$
\boxed{\mathcal A(\epsilon_\ell\to q_\ell)=0\quad\text{for each }\ell=1,2,3.}
$$

Individual [Feynman diagrams](../../../perturbative-quantum-field-theory.md#feynman-diagram) generally fail this test; their complete sum is essential. By linearity in each [photon polarization vector](../../../quantum-mechanics.md#photon-polarization-vector), the result also proves $\mathcal A(\epsilon_\ell+cq_\ell)=\mathcal A(\epsilon_\ell)$. **The amplitude is gauge invariant:** a pure-gauge external [photon](../../../quantum-mechanics.md#photon) polarization decouples, and the physical [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude) depends only on the two transverse [photon](../../../quantum-mechanics.md#photon) polarizations. This is the tree-level [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity) for this process in [quantum electrodynamics](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
