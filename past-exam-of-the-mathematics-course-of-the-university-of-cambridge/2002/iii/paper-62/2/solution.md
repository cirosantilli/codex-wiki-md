<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the [complex scalar field](../../../../../complex-scalar-field.md), the [canonical momenta](../../../../../canonical-momentum.md) are $\pi=\dot\phi^\dagger$ and $\pi^\dagger=\dot\phi$. Split $H=H_0+H_I$. The [interaction picture](../../../../../interaction-picture.md) is obtained from the [Schrödinger picture](../../../../../schrodinger-picture.md) by $|\Psi_I(t)\rangle=e^{iH_0t}|\Psi_S(t)\rangle$ and $O_I(t)=e^{iH_0t}O_Se^{-iH_0t}$, choosing a common time origin. The fields therefore obey the free [Klein-Gordon equation](../../../../../klein-gordon-equation.md), while the states evolve through $H_I(t)$. The [canonical quantization of a complex scalar field](../../../../../canonical-quantization-of-a-complex-scalar-field.md) gives

$$
\phi_I(x)=\int d\Pi_p\,[a(p)e^{-ip\cdot x}+b^\dagger(p)e^{ip\cdot x}],\qquad d\Pi_p=\frac{d^3p}{(2\pi)^3 2E_p}.
$$

The adjoint expansion contains $a^\dagger$ and $b$. Particle and [antiparticle](../../../../../antiparticle.md) modes are independent; their nonzero [commutators](../../../../../commutator.md) are

$$
\boxed{[a(p),a^\dagger(q)]=[b(p),b^\dagger(q)]=(2\pi)^3 2E_p\delta^{(3)}(\mathbf p-\mathbf q).}
$$

All cross-species [commutators](../../../../../commutator.md), and all pairs of [creation operators](../../../../../creation-operator.md) or of [annihilation operators](../../../../../annihilation-operator.md), vanish. These formulas reproduce $[\phi(\mathbf x),\pi(\mathbf y)]=[\phi^\dagger(\mathbf x),\pi^\dagger(\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y)$ and the remaining vanishing equal-time [commutators](../../../../../commutator.md).

There are no derivative interactions, so the [interaction Hamiltonian](../../../../../interaction-hamiltonian.md) is $H_I(t)=-\int d^3x\,\mathcal L_I(x)$. Differentiating the [interaction picture](../../../../../interaction-picture.md) state gives $i\partial_t|\Psi_I\rangle=H_I(t)|\Psi_I\rangle$. Its [time-evolution operator](../../../../../time-evolution-operator.md) satisfies

$$
U(t,t_0)=I-i\int_{t_0}^t dt_1\,H_I(t_1)U(t_1,t_0).
$$

Iteration gives ordered integration regions $t_1>\cdots>t_n$. Each is $1/n!$ of the full region with a [time-ordered product](../../../../../time-ordered-product.md), yielding the [Dyson series](../../../../../dyson-series.md)

$$
U(t,t_0)=\sum_{n=0}^\infty\frac{(-i)^n}{n!}\int_{t_0}^t dt_1\cdots dt_n\,T[H_I(t_1)\cdots H_I(t_n)].
$$

With the usual asymptotic scattering prescription, taking $t_0\to-\infty$ and $t\to+\infty$ proves

$$
\boxed{S=T\exp\!\left(i\int d^4x\,\mathcal L_I(x)\right).}
$$

[Time ordering](../../../../../time-ordering.md) is essential because different interaction Hamiltonians need not commute.

At first order, use the connected tree [scattering amplitude](../../../../../scattering-amplitude.md), equivalently the [normal-ordered](../../../../../normal-ordering.md) quartic vertex with the vacuum and one-particle mass contributions removed. This qualification matters if the local product is interpreted literally without [normal ordering](../../../../../normal-ordering.md): single-vertex [tadpole diagrams](../../../../../tadpole-diagram.md) and [vacuum diagrams](../../../../../vacuum-feynman-diagram.md) are not the requested connected two-particle amplitude. The [complex scalar quartic contact vertex](../../../../../complex-scalar-quartic-contact-vertex.md) is obtained from

$$
S-I=-\frac{i\lambda}{4}\int d^4x\,:\!\phi^{\dagger 2}(x)\phi^2(x)\!:+O(\lambda^2).
$$

In a fully connected matrix element, an incoming particle and outgoing antiparticle attach to the two $\phi$ factors; an outgoing particle and incoming antiparticle attach to the two $\phi^\dagger$ factors. Each pair has two assignments, giving $2!2!=4$. The external [relativistic normalization of a one-particle state](../../../../../relativistic-normalization-of-a-one-particle-state.md) cancels each mode measure: for example $[\phi(x),a^\dagger(p_1)]=e^{-ip_1x}$ and $[b(q_2),\phi(x)]=e^{iq_2x}$. Consequently the connected integrand is $4e^{-i(p_1+q_1-p_2-q_2)\cdot x}$, and

$$
\langle p_2q_2|(S-I)|p_1q_1\rangle_{\rm conn}
=-i\lambda(2\pi)^4\delta^{(4)}(p_1+q_1-p_2-q_2)+O(\lambda^2).
$$

Thus **the invariant connected amplitude is**

$$
\boxed{\mathcal T=-\lambda+O(\lambda^2).}
$$

The [Dirac delta function](../../../../../dirac-delta-function.md) expresses [four-momentum conservation](../../../../../four-momentum-conservation.md).

For the identity contribution, commute $a(p_2)$ through $a^\dagger(p_1)$ and independently $b(q_2)$ through $b^\dagger(q_1)$; all terms leaving a [creation operator](../../../../../creation-operator.md) against the left [Fock vacuum](../../../../../fock-vacuum.md) or an [annihilation operator](../../../../../annihilation-operator.md) against the right [Fock vacuum](../../../../../fock-vacuum.md) vanish. Hence

$$
\boxed{\langle p_2q_2|I|p_1q_1\rangle=(2\pi)^6(2E_{p_1})(2E_{q_1})\delta^{(3)}(\mathbf p_2-\mathbf p_1)\delta^{(3)}(\mathbf q_2-\mathbf q_1).}
$$

There is no exchange term between the two distinct particle and [antiparticle](../../../../../antiparticle.md) species.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
