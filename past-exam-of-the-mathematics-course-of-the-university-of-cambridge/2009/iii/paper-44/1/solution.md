<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use natural units $\hbar=c=1$ and the [Minkowski metric](../../../../../minkowski-metric.md) $g=\operatorname{diag}(1,-1,-1,-1)$. The [canonical momentum](../../../../../canonical-momentum.md) is $\pi=\partial\mathcal L/\partial\dot\phi=\dot\phi$, and the [Legendre transform in mechanics](../../../../../legendre-transform-in-mechanics.md) gives

$$
H=\frac12\int d^3x\,[\pi^2+(\nabla\phi)^2+m^2\phi^2].
$$

For [canonical quantization of a real scalar field](../../../../../canonical-quantization-of-a-real-scalar-field.md), impose the equal-time [canonical commutation relations](../../../../../canonical-commutation-relation.md)

$$
[\phi(t,\mathbf x),\pi(t,\mathbf y)]=i\delta^3(\mathbf x-\mathbf y),\qquad
[\phi(t,\mathbf x),\phi(t,\mathbf y)]=[\pi(t,\mathbf x),\pi(t,\mathbf y)]=0.
$$

The [Heisenberg picture](../../../../../heisenberg-picture.md) equation $\dot O=i[H,O]$ then gives $\dot\phi=\pi$. For the other equation, the momentum term commutes with $\pi$; commuting the gradient term past $\pi$ and integrating the derivative of the [Dirac delta function](../../../../../dirac-delta-function.md) by parts gives $\dot\pi=\nabla^2\phi-m^2\phi$. Consequently

$$
\boxed{(\Box+m^2)\phi=0,\qquad\Box=\partial_t^2-\nabla^2.}
$$

The [Fourier transform](../../../../../fourier-transform.md) reduces this [Klein-Gordon equation](../../../../../klein-gordon-equation.md) to oscillators of frequency $E_{\mathbf p}=\sqrt{\mathbf p^2+m^2}$. Hermiticity of the [real scalar field](../../../../../real-scalar-field.md) pairs their positive- and negative-frequency coefficients, so its general mode expansion can be normalized as

$$
\phi(x)=\int\frac{d^3p}{(2\pi)^3\sqrt{2E_{\mathbf p}}}
[a(\mathbf p)e^{-ip\cdot x}+a^\dagger(\mathbf p)e^{ip\cdot x}],\qquad p^0=E_{\mathbf p}.
$$

To verify its normalization rather than guess the oscillator algebra, use [scalar field oscillator inversion](../../../../../scalar-field-oscillator-inversion.md) at $t=0$:

$$
a(\mathbf p)=\int d^3x\,e^{-i\mathbf p\cdot\mathbf x}
\left[\sqrt{E_{\mathbf p}/2}\,\phi(0,\mathbf x)+\frac{i}{\sqrt{2E_{\mathbf p}}}\pi(0,\mathbf x)\right].
$$

Its adjoint has the conjugate phase and the opposite sign in front of $i\pi$. The two mixed field-momentum [commutators](../../../../../commutator.md) give

$$
[a(\mathbf p),a^\dagger(\mathbf q)]
=\frac{E_{\mathbf p}+E_{\mathbf q}}{2\sqrt{E_{\mathbf p}E_{\mathbf q}}}
\int d^3x\,e^{i(\mathbf q-\mathbf p)\cdot\mathbf x}
=\boxed{(2\pi)^3\delta^3(\mathbf p-\mathbf q)}.
$$

The [Fourier representation of the Dirac delta function](../../../../../fourier-representation-of-the-dirac-delta-function.md) sets the energies equal in the last step. Similarly, $[a(\mathbf p),a(\mathbf q)]$ has a factor $E_{\mathbf q}-E_{\mathbf p}$ multiplying $\delta^3(\mathbf p+\mathbf q)$ and vanishes; the two-creator commutator vanishes as well.

Substituting the expansion in $H$ and integrating the spatial phases, the two-annihilator and two-creator coefficients cancel by $E_{\mathbf p}^2=\mathbf p^2+m^2$. The [free real scalar Hamiltonian in oscillator variables](../../../../../free-real-scalar-hamiltonian-in-oscillator-variables.md) is

$$
H=\frac12\int\frac{d^3p}{(2\pi)^3}E_{\mathbf p}
[a^\dagger(\mathbf p)a(\mathbf p)+a(\mathbf p)a^\dagger(\mathbf p)].
$$

It differs from $:H:=\int d^3p\,E_{\mathbf p}a^\dagger a/(2\pi)^3$ by its constant [vacuum energy](../../../../../vacuum-energy.md); [normal ordering](../../../../../normal-ordering.md) removes that constant. Using the oscillator commutators, for either Hamiltonian,

$$
\boxed{[H,a(\mathbf p)]=-E_{\mathbf p}a(\mathbf p),\qquad
[H,a^\dagger(\mathbf p)]=E_{\mathbf p}a^\dagger(\mathbf p).}
$$

Choose the [Fock vacuum](../../../../../fock-vacuum.md) annihilated by every $a(\mathbf p)$. Each [creation operator](../../../../../creation-operator.md) adds a particle of energy $E_{\mathbf p}$ and momentum $\mathbf p$; its [annihilation operator](../../../../../annihilation-operator.md) removes one. Their mutual commutativity gives [bosonic Fock space](../../../../../bosonic-fock-space.md) and symmetric many-particle states. Thus the scalar mass-shell frequency has a particle interpretation, rather than merely describing a classical oscillation.

For $t=x^0-y^0$ and $\mathbf r=\mathbf x-\mathbf y$, vacuum contraction and [time ordering](../../../../../time-ordering.md) give the [Feynman propagator](../../../../../feynman-propagator.md)

$$
D_F(t,\mathbf r)=\int\frac{d^3p}{(2\pi)^3}\frac{e^{i\mathbf p\cdot\mathbf r}}{2E_{\mathbf p}}
[\theta(t)e^{-iE_{\mathbf p}t}+\theta(-t)e^{iE_{\mathbf p}t}].
$$

In the [scalar Feynman propagator pole prescription](../../../../../scalar-feynman-propagator-pole-prescription.md), the integral of $i e^{-ip^0t}/((p^0)^2-E_{\mathbf p}^2+i0)$ has poles at $E_{\mathbf p}-i0$ and $-E_{\mathbf p}+i0$. Close clockwise below for $t>0$ and counterclockwise above for $t<0$. The [residue theorem](../../../../../residue-theorem.md) gives exactly the corresponding term above, proving

$$
\boxed{D_F(x-y)=\int\frac{d^4p}{(2\pi)^4}\frac{i\,e^{-ip\cdot(x-y)}}{p^2-m^2+i0}.}
$$

As a direct check of the distributional source, $g_E(t)=e^{-iE|t|}/(2E)$ is continuous, but $g'_E(0^+)-g'_E(0^-)=-i$. The [derivative jump of a free scalar time-ordered two-point function](../../../../../derivative-jump-of-a-free-scalar-time-ordered-two-point-function.md) therefore gives $(\partial_t^2+E^2)g_E=-i\delta(t)$. Spatial Fourier inversion yields

$$
\boxed{(\Box+m^2)D_F(x-y)=-i\delta^4(x-y).}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
