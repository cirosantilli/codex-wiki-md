<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use units $\hbar=c=1$, metric $g_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$, and $p\cdot x=E_{\mathbf p}t-\mathbf p\cdot\mathbf x$. Treat the [complex scalar field](../../../../../complex-scalar-field.md) and its adjoint as independent variables when varying the [action](../../../../../action.md). Their [canonical momenta](../../../../../canonical-momentum.md) are

$$
\boxed{\pi=\frac{\partial\mathcal L}{\partial\dot\phi}=\dot\phi^\dagger,\qquad
\pi^\dagger=\frac{\partial\mathcal L}{\partial\dot\phi^\dagger}=\dot\phi.}
$$

[Canonical quantization](../../../../../canonical-quantization.md) in the [Heisenberg picture](../../../../../heisenberg-picture.md) imposes, at the same time $t$,

$$
[\phi(t,\mathbf x),\pi(t,\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y),\qquad
[\phi^\dagger(t,\mathbf x),\pi^\dagger(t,\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y).
$$

All other independent equal-time commutators vanish: in particular $[\phi,\phi^\dagger]=[\pi,\pi^\dagger]=[\phi,\pi^\dagger]=[\phi^\dagger,\pi]=0$, together with the same-type field and momentum commutators. The [Legendre transform](../../../../../convex-conjugate.md) gives the [Hamiltonian density](../../../../../hamiltonian-density.md)

$$
\boxed{\mathcal H=\pi\dot\phi+\pi^\dagger\dot\phi^\dagger-\mathcal L
=\pi\pi^\dagger+\nabla\phi^\dagger\cdot\nabla\phi+m^2\phi^\dagger\phi,\qquad H=\int d^3x\,\mathcal H.}
$$

The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) are $(\Box+m^2)\phi=(\Box+m^2)\phi^\dagger=0$. The positive- and negative-frequency [plane waves](../../../../../plane-wave.md) form a complete basis of solutions of the [Klein-Gordon equation](../../../../../klein-gordon-equation.md). Since the field is complex, their operator coefficients are independent rather than being adjoints of each other. Define the [Lorentz-invariant phase space](../../../../../lorentz-invariant-phase-space.md) measure $d\Pi_p=d^3\mathbf p/[(2\pi)^3 2E_{\mathbf p}]$. A convenient expansion is

$$
\phi(x)=\int d\Pi_p\left[a(\mathbf p)e^{-ip\cdot x}-b^\dagger(\mathbf p)e^{ip\cdot x}\right],\qquad
\phi^\dagger(x)=\int d\Pi_p\left[a^\dagger(\mathbf p)e^{ip\cdot x}-b(\mathbf p)e^{-ip\cdot x}\right].
$$

The minus sign is a phase convention: replacing $b$ by $-b$ produces the usual plus-sign expansion without changing its commutators or [number operator](../../../../../number-operator.md). The normalization is fixed by the [canonical commutation relations](../../../../../canonical-commutation-relation.md). For example,

$$
\begin{aligned}
\pi(x)&=i\int d\Pi_p\,E_{\mathbf p}\left[a^\dagger(\mathbf p)e^{ip\cdot x}+b(\mathbf p)e^{-ip\cdot x}\right],\\
[\phi(t,\mathbf x),\pi(t,\mathbf y)]
&=\frac i2\int\frac{d^3\mathbf p}{(2\pi)^3}
\left[e^{i\mathbf p\cdot(\mathbf x-\mathbf y)}+e^{-i\mathbf p\cdot(\mathbf x-\mathbf y)}\right]
=i\delta^{(3)}(\mathbf x-\mathbf y),
\end{aligned}
$$

when $[a(\mathbf p),a^\dagger(\mathbf q)]=[b(\mathbf p),b^\dagger(\mathbf q)]=(2\pi)^3 2E_{\mathbf p}\delta^{(3)}(\mathbf p-\mathbf q)$. The cross commutators vanish and the other canonical relation follows by taking adjoints with the operator order reversed. Conversely these mode commutators can be obtained by Fourier inversion of the equal-time relations. This is [canonical quantization of a complex scalar field](../../../../../canonical-quantization-of-a-complex-scalar-field.md).

Substitution into the spatial integral for $H$ makes the diagonal terms proportional to $a^\dagger a$ and $bb^\dagger$. Terms creating or annihilating a pair have $\mathbf q=-\mathbf p$ and a coefficient $E_{\mathbf p}^2-\mathbf p^2-m^2=0$, so they cancel. The result before vacuum subtraction is

$$
H_{\rm raw}=\int d\Pi_p\,E_{\mathbf p}\left[a^\dagger(\mathbf p)a(\mathbf p)+b(\mathbf p)b^\dagger(\mathbf p)\right].
$$

Commuting $b$ past $b^\dagger$ leaves a divergent field-independent [vacuum energy](../../../../../vacuum-energy.md). The displayed zero-vacuum-energy form must therefore be understood as a [normal-ordered](../../../../../normal-ordering.md) [Hamiltonian](../../../../../hamiltonian.md):

$$
\boxed{H=:H_{\rm raw}:=\int d\Pi_p\,E_{\mathbf p}(a^\dagger a+b^\dagger b)
=\int\frac{d^3\mathbf p}{(2\pi)^3}\frac12(a^\dagger a+b^\dagger b).}
$$

A regulator can be introduced before subtracting the constant. This is the [normal-ordered Hamiltonian of a free complex scalar field](../../../../../normal-ordered-hamiltonian-of-a-free-complex-scalar-field.md); the unrenormalized [Hamiltonian](../../../../../hamiltonian.md) is not literally equal to this expression without that convention.

The [scalar-field vacuum](../../../../../scalar-field-vacuum.md) is annihilated by both [annihilation operators](../../../../../annihilation-operator.md). Their adjoints create two species of [spin](../../../../../spin.md)-zero [bosons](../../../../../boson.md) with the same positive energy $E_{\mathbf p}$ and [mass](../../../../../mass.md) $m$, because

$$
[H,a^\dagger(\mathbf p)]=E_{\mathbf p}a^\dagger(\mathbf p),\qquad
[H,b^\dagger(\mathbf p)]=E_{\mathbf p}b^\dagger(\mathbf p).
$$

Repeated [creation operators](../../../../../creation-operator.md) give the bosonic [Fock space](../../../../../fock-space.md). The negative-frequency part does not create a negative-energy physical state; it creates the [antiparticle](../../../../../antiparticle.md) of positive energy. The charge distinguishes the two species.

For the global phase transformation $\delta\phi=-i\alpha\phi$, $\delta\phi^\dagger=i\alpha\phi^\dagger$, [Noether theorem](../../../../../noether-theorem.md) gives $j^\mu=i(\phi^\dagger\partial^\mu\phi-\partial^\mu\phi^\dagger\,\phi)$. Its divergence is

$$
\partial_\mu j^\mu=i(\phi^\dagger\Box\phi-\Box\phi^\dagger\,\phi)
=i(-m^2\phi^\dagger\phi+m^2\phi^\dagger\phi)=0.
$$

With vanishing boundary flux, the integral of $j^0$ is a [conserved charge](../../../../../conserved-charge.md). Substituting the modes gives, before charge [normal ordering](../../../../../normal-ordering.md), $Q_{\rm raw}=\int d\Pi_p(a^\dagger a-bb^\dagger)$. The pair terms cancel because their frequency difference is zero when their spatial momenta sum to zero. Taking the vacuum charge to vanish gives the [complex scalar charge operator](../../../../../complex-scalar-charge-operator.md)

$$
\boxed{Q=\int d\Pi_p(a^\dagger a-b^\dagger b).}
$$

The mode commutators imply $[Q,a^\dagger]=a^\dagger$ and $[Q,b^\dagger]=-b^\dagger$, so

$$
\boxed{Qa^\dagger=a^\dagger(Q+1),\qquad Qb^\dagger=b^\dagger(Q-1).}
$$

Thus the particle carries charge $+1$, the [antiparticle](../../../../../antiparticle.md) carries charge $-1$, and a state with occupation numbers $n_a,n_b$ has charge $n_a-n_b$. Also $[Q,\phi]=-\phi$ and $[Q,H]=0$, agreeing with the phase transformation and charge conservation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
