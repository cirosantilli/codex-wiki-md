<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Treat $\phi,\phi^\dagger$ as independent variables when taking the [Legendre transform](../../../../../convex-conjugate.md). Their [canonical momenta](../../../../../canonical-momentum.md) are

$$
\boxed{\pi=\frac{\partial\mathcal L}{\partial\dot\phi}=\dot\phi^\dagger,\qquad
\pi^\dagger=\frac{\partial\mathcal L}{\partial\dot\phi^\dagger}=\dot\phi.}
$$

The [canonical quantization of a complex scalar field](../../../../../canonical-quantization-of-a-complex-scalar-field.md) imposes, at equal times,

$$
\begin{aligned}
[\phi(t,\mathbf x),\pi(t,\mathbf y)]&=i\delta^3(\mathbf x-\mathbf y),\\
[\phi^\dagger(t,\mathbf x),\pi^\dagger(t,\mathbf y)]&=i\delta^3(\mathbf x-\mathbf y),
\end{aligned}
$$

with $[\phi,\phi^\dagger]=[\phi,\phi]=[\pi,\pi^\dagger]=[\pi,\pi]=0$, together with their adjoints, and $[\phi,\pi^\dagger]=[\phi^\dagger,\pi]=0$. These are [canonical commutation relations](../../../../../canonical-commutation-relation.md) for two real scalar degrees of freedom, written in a complex basis. Local fields are [operator-valued distributions](../../../../../operator-valued-distribution.md), so these identities are understood after smearing or with a regulator.

The [Hamiltonian density](../../../../../hamiltonian-density.md) is $\pi\dot\phi+\pi^\dagger\dot\phi^\dagger-\mathcal L$, giving

$$
\boxed{H=\int d^3x\left(\pi^\dagger\pi+\nabla\phi^\dagger\cdot\nabla\phi+m^2\phi^\dagger\phi\right).}
$$

The [Heisenberg equation of motion](../../../../../heisenberg-equation-of-motion.md) is $\dot O=i[H,O]$. For example, $i[\int\pi^\dagger\pi,\phi]=\pi^\dagger$, while commuting $\pi$ with the gradient term and integrating its derivative of a [Dirac delta distribution](../../../../../dirac-delta-function.md) gives $\nabla^2\phi^\dagger$. Thus

$$
\boxed{\dot\phi=\pi^\dagger,\quad\dot\phi^\dagger=\pi,\quad
\dot\pi^\dagger=(\nabla^2-m^2)\phi,\quad\dot\pi=(\nabla^2-m^2)\phi^\dagger.}
$$

Both fields satisfy the [Klein-Gordon equation](../../../../../klein-gordon-equation.md). Their spatial [Fourier modes](../../../../../fourier-mode.md) therefore have [frequencies](../../../../../frequency.md) $\pm E_p$, $E_p=\sqrt{\mathbf p^2+m^2}$. A [complex scalar field](../../../../../complex-scalar-field.md) has independent [coefficients](../../../../../coefficient.md) for these two [frequency](../../../../../frequency.md) sectors, so, defining the invariant measure $d\Pi_p=d^3p/[(2\pi)^3 2E_p]$, its mode expansion is

$$
\phi(x)=\int d\Pi_p\left[a(p)e^{-ip\cdot x}+b^\dagger(p)e^{ip\cdot x}\right],\qquad p^0=E_p>0.
$$

One can recover the mode operators at any fixed time using [complex scalar mode inversion](../../../../../complex-scalar-mode-inversion.md):

$$
a(p)=\int d^3x\,e^{ip\cdot x}(E_p\phi+i\dot\phi),\qquad
b^\dagger(p)=\int d^3x\,e^{-ip\cdot x}(E_p\phi-i\dot\phi).
$$

Substitution of the expansion verifies these inverses: the spatial integral selects the appropriate [momentum](../../../../../momentum.md), while the two [frequency](../../../../../frequency.md) sectors acquire factors $E_p\pm E_q$. The unwanted sector vanishes when the delta function sets $E_p=E_q$. The [canonical commutation relations](../../../../../canonical-commutation-relation.md) then give, for example,

$$
[a(p),a^\dagger(q)]=(E_p+E_q)(2\pi)^3\delta^3(\mathbf p-\mathbf q)
=(2\pi)^3 2E_p\delta^3(\mathbf p-\mathbf q).
$$

Likewise $[b(p),b^\dagger(q)]$ has the same value. The cross commutators vanish; their [coefficients](../../../../../coefficient.md) contain $E_p-E_q$ on the corresponding [momentum](../../../../../momentum.md) delta function. Conversely, these oscillator brackets reproduce the equal-time field brackets, confirming the normalization of the measure.

Insert the mode expansion into $H$ and integrate over space. The terms $a^\dagger b^\dagger$ and $ba$ enforce opposite spatial [momenta](../../../../../momentum.md); their [coefficient](../../../../../coefficient.md) is $-E_p^2+\mathbf p^2+m^2=0$. For the diagonal terms the [coefficient](../../../../../coefficient.md) is $E_p^2+\mathbf p^2+m^2=2E_p^2$. Combining this with the two invariant measures leaves

$$
H_{\rm bare}=\int d\Pi_p\,E_p\left[a^\dagger(p)a(p)+b(p)b^\dagger(p)\right]
=H_{\rm normal}+E_0I.
$$

In a box, $E_0=\sum_{\mathbf p}E_p$, one half-quantum for each of the two real oscillator species. It diverges as the cutoff is removed. [Normal ordering](../../../../../normal-ordering.md) removes this [vacuum energy](../../../../../vacuum-energy.md), yielding the [normal-ordered Hamiltonian of a free complex scalar field](../../../../../normal-ordered-hamiltonian-of-a-free-complex-scalar-field.md):

$$
\boxed{H_{\rm normal}=\int d\Pi_p\,E_p[a^\dagger(p)a(p)+b^\dagger(p)b(p)].}
$$

In this nongravitational free theory an additive constant in $H$ changes only an overall state phase, not [Heisenberg equations of motion](../../../../../heisenberg-equation-of-motion.md), [energy](../../../../../energy.md) differences or scattering probabilities. It is therefore consistent to choose the [Fock vacuum](../../../../../fock-vacuum.md) [energy](../../../../../energy.md) as zero. Both [creation operators](../../../../../creation-operator.md) raise the [energy](../../../../../energy.md): $[H,a^\dagger(p)]=E_pa^\dagger(p)$ and $[H,b^\dagger(p)]=E_pb^\dagger(p)$. Repeated creation builds a [bosonic Fock space](../../../../../bosonic-fock-space.md) of spin-zero particles and antiparticles, with the same positive mass and [energy](../../../../../energy.md). The negative-frequency part of the field does not describe negative-energy physical particles.

The [global phase symmetry of a complex scalar field](../../../../../global-phase-symmetry-of-a-complex-scalar-field.md), with orientation $\phi\mapsto e^{-i\alpha}\phi$, has the indicated [Noether current](../../../../../noether-current.md). Taking its divergence, the two first-derivative terms cancel, giving

$$
\partial_\mu J^\mu=i\left(\phi^\dagger\Box\phi-(\Box\phi^\dagger)\phi\right)
=i[-m^2\phi^\dagger\phi+m^2\phi^\dagger\phi]=\boxed{0}.
$$

The same calculation holds for its [normal-ordered](../../../../../normal-ordering.md) version. Integrating its temporal component gives a conserved charge when spatial boundary flux vanishes.

Here the ordering convention is important. Direct substitution into the literally ordered product $i\int(\phi^\dagger\dot\phi-\dot\phi^\dagger\phi)d^3x$ yields

$$
Q_{\rm bare}=\int d\Pi_p\left[a^\dagger(p)a(p)-b(p)b^\dagger(p)\right].
$$

The pair terms again vanish, now because their [coefficient](../../../../../coefficient.md) is a difference of equal [energies](../../../../../energy.md). Reordering the $b$ term produces a divergent vacuum constant: with a finite-mode regulator $Q_{\rm bare}=N_a-N_b-N_{\rm modes}$. Thus the requested finite charge formula uses **zero vacuum charge**, or equivalently the [vacuum subtraction of a complex scalar charge](../../../../../vacuum-subtraction-of-a-complex-scalar-charge.md). With that conventional subtraction,

$$
\boxed{Q=\int d\Pi_p\left[a^\dagger(p)a(p)-b^\dagger(p)b(p)\right],\qquad Q|0\rangle=0.}
$$

The subtraction changes neither current conservation nor the action of $Q$ on fields; without it, the unrenormalized product does not literally equal the displayed [normal-ordered](../../../../../normal-ordering.md) operator.

Finally the oscillator commutators give

$$
[Q,a^\dagger(p)]=a^\dagger(p),\qquad [Q,b^\dagger(p)]=-b^\dagger(p),
$$

or $\boxed{Qa^\dagger=a^\dagger(Q+1),\quad Qb^\dagger=b^\dagger(Q-1)}$. Acting on a charge eigenstate, the first creator raises its charge by one and the second lowers it by one. Starting from the neutral [Fock vacuum](../../../../../fock-vacuum.md), their one-particle states therefore have charges **$+1$ and $-1$ respectively**. This is the [complex scalar charge operator](../../../../../complex-scalar-charge-operator.md) $N_a-N_b$, whereas the [energy](../../../../../energy.md) counts the sum of the two occupations. A multiparticle state has additive charge equal to the number of particles minus the number of antiparticles.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
