<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use units $\hbar=c=1$ and the [Minkowski metric](../../../../../minkowski-metric.md) $g=\operatorname{diag}(1,-1,-1,-1)$. The [canonical momentum](../../../../../canonical-momentum.md) of the [real scalar field](../../../../../real-scalar-field.md) is $\pi=\partial\mathcal L/\partial\dot\phi=\dot\phi$. [Canonical quantization](../../../../../canonical-quantization.md) replaces the classical fields by [operator-valued distributions](../../../../../operator-valued-distribution.md) and imposes the equal-time [canonical commutation relations](../../../../../canonical-commutation-relation.md)

$$
[\phi(t,\mathbf x),\pi(t,\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y),\qquad [\phi(t,\mathbf x),\phi(t,\mathbf y)]=[\pi(t,\mathbf x),\pi(t,\mathbf y)]=0.
$$

These relations are imposed on an initial slice, with smeared fields understood. In the [Heisenberg picture](../../../../../heisenberg-picture.md), simultaneous [unitary time evolution](../../../../../unitary-time-evolution.md) of both operators preserves their [commutators](../../../../../commutator.md). Since the momentum is $\dot\phi$, **the requested equal-time commutator is** $[\phi(t,\mathbf x),\dot\phi(t,\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y)$.

The [Legendre transform in mechanics](../../../../../legendre-transform-in-mechanics.md), applied pointwise, gives the [canonical Hamiltonian density of a real scalar field](../../../../../canonical-hamiltonian-density-of-a-real-scalar-field.md). Thus

$$
\boxed{H=\frac12\int d^3x\,[\pi^2+|\nabla\phi|^2+m^2\phi^2].}
$$

To obtain its dynamics rather than assume them, use the [Heisenberg equation of motion](../../../../../heisenberg-equation-of-motion.md) $\dot O=i[H,O]$. The momentum-square term gives $[H,\phi]=-i\pi$. The field-square term gives $[H,\pi]=im^2\phi$, while differentiating the [Dirac delta function](../../../../../dirac-delta-function.md) in the gradient term and integrating by parts gives $[H,\pi]=-i\nabla^2\phi+im^2\phi$. Consequently

$$
\dot\phi=\pi,\qquad \dot\pi=\nabla^2\phi-m^2\phi,\qquad \boxed{(\Box+m^2)\phi=0.}
$$

Boundary terms vanish for suitably decaying smeared fields. This is the [Klein-Gordon equation](../../../../../klein-gordon-equation.md) as an operator identity.

A spatial [Fourier transform](../../../../../fourier-transform.md) reduces the [Klein-Gordon equation](../../../../../klein-gordon-equation.md) to $\ddot\phi_{\mathbf p}+E_p^2\phi_{\mathbf p}=0$, where $E_p=\sqrt{\mathbf p^2+m^2}$. Its two frequency branches and the [Hermitian adjoint](../../../../../adjoint-operator.md) condition give

$$
\phi(x)=\int d\Pi_p\,[a(p)e^{-ip\cdot x}+a^\dagger(p)e^{ip\cdot x}],\qquad d\Pi_p=\frac{d^3p}{(2\pi)^3 2E_p},\quad p^0=E_p.
$$

The [invariant-normalized scalar mode extraction](../../../../../invariant-normalized-scalar-mode-extraction.md) can be written particularly simply as

$$
a(p)=\int d^3x\,e^{ip\cdot x}[E_p\phi(x)+i\pi(x)],\qquad a^\dagger(p)=\int d^3x\,e^{-ip\cdot x}[E_p\phi(x)-i\pi(x)].
$$

Substituting the [mode expansion of a free field](../../../../../mode-expansion-of-a-free-field.md) proves these inversion formulas: the opposite-frequency coefficient is proportional to $E_p-E_q$ and vanishes after spatial [Fourier inversion](../../../../../fourier-inversion-theorem.md). Alternatively they are the corresponding [Klein-Gordon inner products](../../../../../klein-gordon-inner-product.md). Taking their [commutators](../../../../../commutator.md) using the equal-time fields gives $(E_p+E_q)(2\pi)^3\delta^{(3)}(\mathbf p-\mathbf q)$ in the mixed case. In the two equal-type cases the delta function enforces $\mathbf q=-\mathbf p$, multiplying $E_p-E_q=0$. Therefore

$$
\boxed{[a(p),a^\dagger(q)]=(2\pi)^3 2E_p\delta^{(3)}(\mathbf p-\mathbf q),\qquad [a(p),a(q)]=[a^\dagger(p),a^\dagger(q)]=0.}
$$

Conversely these mode [commutators](../../../../../commutator.md) reproduce $[\phi,\dot\phi]=i\delta^{(3)}$: the two frequency contributions each supply half the spatial [Dirac delta function](../../../../../dirac-delta-function.md).

For the [covariant oscillator Hamiltonian of a real scalar field](../../../../../covariant-oscillator-hamiltonian-of-a-real-scalar-field.md), insert the [mode expansion of a free field](../../../../../mode-expansion-of-a-free-field.md) into $H$. Spatial integration sets the two momenta equal in the mixed terms and opposite in the two-creator or two-annihilator terms. The latter have coefficient $-E_p^2+\mathbf p^2+m^2=0$. The mixed terms give

$$
H=\frac12\int d\Pi_p\,E_p[a^\dagger(p)a(p)+a(p)a^\dagger(p)]
=\int d\Pi_p\,E_p a^\dagger(p)a(p)+E_0,
\qquad E_0=\frac12\int d^3p\,E_p\delta^{(3)}(0).
$$

The constant $E_0$ is the divergent [zero-point energy](../../../../../zero-point-energy.md); a finite box and a momentum cutoff make its meaning explicit. [Normal ordering](../../../../../normal-ordering.md) sets the free [vacuum energy](../../../../../vacuum-energy.md) to zero and leaves all [commutators](../../../../../commutator.md) unchanged. Directly applying the mode [commutators](../../../../../commutator.md) to the mixed expression yields

$$
\boxed{[H,a(p)]=-E_pa(p),\qquad [H,a^\dagger(p)]=E_pa^\dagger(p).}
$$

Choose the [Fock vacuum](../../../../../fock-vacuum.md) by $a(p)|0\rangle=0$. Each [creation operator](../../../../../creation-operator.md) adds a [boson](../../../../../boson.md) of energy $E_p$ and [four-momentum](../../../../../four-momentum.md) $p$, while each [annihilation operator](../../../../../annihilation-operator.md) removes one. Products of commuting [creation operators](../../../../../creation-operator.md) give [bosonic statistics from commuting creation operators](../../../../../bosonic-statistics-from-commuting-creation-operators.md) and unrestricted [occupation numbers](../../../../../occupation-number.md). The [real scalar field](../../../../../real-scalar-field.md) has one spin-zero species, identical to its [antiparticle](../../../../../antiparticle.md). Its [one-particle states](../../../../../one-particle-state.md) obey $\langle q|p\rangle=(2\pi)^3 2E_p\delta^{(3)}(\mathbf p-\mathbf q)$, precisely the [relativistic normalization of a one-particle state](../../../../../relativistic-normalization-of-a-one-particle-state.md).

For the [Feynman propagator](../../../../../feynman-propagator.md), put $z=x-y$ and contract the two fields in the [Fock vacuum](../../../../../fock-vacuum.md). Only $aa^\dagger$ survives, giving the [Wightman function](../../../../../wightman-function.md)

$$
W(z)=\langle0|\phi(x)\phi(y)|0\rangle=\int d\Pi_p\,e^{-ip\cdot z}.
$$

The stipulated [time-ordered product](../../../../../time-ordered-product.md) convention is $i\Delta_F(z)=\theta(z^0)W(z)+\theta(-z^0)W(-z)$. In a [contour integral](../../../../../contour-integral.md) over $p^0$, the [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md) places the positive-energy pole just below the real axis and the negative-energy pole just above it. For $z^0>0$ close below, clockwise, obtaining $-i e^{-iE_pz^0}/(2E_p)$; for $z^0<0$ close above, obtaining $-i e^{iE_pz^0}/(2E_p)$. Changing $\mathbf p\mapsto-\mathbf p$ in the second contribution therefore proves

$$
\boxed{\Delta_F(z)=\lim_{\epsilon\downarrow0}\int\frac{d^4p}{(2\pi)^4}\frac{e^{-ip\cdot z}}{p^2-m^2+i\epsilon}.}
$$

Acting with $\Box+m^2$ multiplies the integrand by $-(p^2-m^2)$. The remaining factor tends to $-1$ as a [distribution](../../../../../distribution-mathematical-analysis.md), so [Fourier inversion](../../../../../fourier-inversion-theorem.md) gives

$$
\boxed{(\Box+m^2)\Delta_F(z)=-\delta^{(4)}(z).}
$$

The sign also follows from the [derivative jump of a free scalar time-ordered two-point function](../../../../../derivative-jump-of-a-free-scalar-time-ordered-two-point-function.md): the first time derivative of $i\Delta_F$ jumps by $\langle[\dot\phi,\phi]\rangle=-i\delta^{(3)}$, so that of $\Delta_F$ jumps by $-\delta^{(3)}$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
