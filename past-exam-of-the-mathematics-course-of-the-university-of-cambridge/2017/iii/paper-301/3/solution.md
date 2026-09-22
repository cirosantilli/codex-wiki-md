<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use a local first-derivative [Lagrangian density](../../../../../lagrangian-density.md) $\mathcal L(\phi,\partial_\mu\phi,x)$ with sufficient [differentiability](../../../../../differentiability.md), and let variations have [compact support](../../../../../compact-support.md) or vanish at the spacetime boundary. If the phrase “a function of the field” were read literally as forbidding derivatives, the equation below would reduce to $\partial\mathcal L/\partial\phi=0$; a propagating field requires derivative dependence. Varying the [action](../../../../../action.md) gives

$$
\delta S=\int d^4x\left(\mathcal L_\phi\delta\phi+\Pi^\mu\partial_\mu\delta\phi\right),\qquad\Pi^\mu=\frac{\partial\mathcal L}{\partial(\partial_\mu\phi)}.
$$

[Integration by parts](../../../../../integration-by-parts.md) and arbitrary interior variations yield the [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md),

$$
\boxed{\mathcal E(\phi):=\mathcal L_\phi-\partial_\mu\Pi^\mu=0.}
$$

The boundary condition is part of this derivation; if boundary variations are allowed, their separate boundary equations must also be imposed.

A [variational symmetry of a Lagrangian density](../../../../../variational-symmetry-of-a-lagrangian-density.md) is an infinitesimal field change $\delta\phi=\varepsilon X$ for which $\delta\mathcal L=\varepsilon\partial_\mu K^\mu$ off shell. Equality to zero is sufficient but is not necessary: a divergence changes only the boundary contribution to the [action](../../../../../action.md). For fixed-coordinate field variations,

$$
\frac{\delta\mathcal L}{\varepsilon}=\mathcal E(\phi)X+\partial_\mu(\Pi^\mu X).
$$

Equating the two expressions proves the scalar-field form of the [Noether theorem](../../../../../noether-theorem.md):

$$
\boxed{j^\mu=\Pi^\mu X-K^\mu,\qquad\partial_\mu j^\mu=-\mathcal E(\phi)X=0\quad\text{on shell}.}
$$

Thus every differentiable one-parameter variational symmetry gives a [conserved current](../../../../../conserved-current.md), and its [Noether charge](../../../../../noether-charge.md) $Q=\int d^3x\,j^0$ is constant when the spatial boundary flux vanishes. This is the [Noether current for a first-derivative scalar field](../../../../../noether-current-for-a-first-derivative-scalar-field.md); the same identity applies to several real components by summing over them. Identically conserved improvement terms can change its local expression without changing the charge under the same boundary assumptions.

For an active spacetime translation, $\phi'(x)=\phi(x-a)$ and $\delta\phi=-a^\nu\partial_\nu\phi$. If the [Lagrangian density](../../../../../lagrangian-density.md) has no explicit coordinate dependence, $\delta\mathcal L=-a^\nu\partial_\nu\mathcal L$, so $K^\mu=-a^\mu\mathcal L$. The [Noether current](../../../../../noether-current.md) is $j^\mu=-a^\nu T^\mu{}_{\nu}$, where

$$
\boxed{T^\mu{}_{\nu}=\Pi^\mu\partial_\nu\phi-\delta^\mu{}_{\nu}\mathcal L,\qquad\partial_\mu T^\mu{}_{\nu}=0.}
$$

These four translation currents are the [canonical stress-energy tensor](../../../../../canonical-stress-energy-tensor.md), also called the energy-momentum tensor. The sign in $j=-aT$ follows from the chosen active translation; the translation charges themselves can be labelled by $P_\nu=\int T^0{}_{\nu}d^3x$.

For the free [real scalar field](../../../../../real-scalar-field.md), take the standard [kinetic term](../../../../../kinetic-term.md) and [mass term](../../../../../mass-term.md). Its [Lagrangian density](../../../../../lagrangian-density.md) and [Klein-Gordon equation](../../../../../klein-gordon-equation.md) are

$$
\mathcal L=\frac12\partial_\mu\phi\partial^\mu\phi-\frac12m^2\phi^2,\qquad
\boxed{(\Box+m^2)\phi=0.}
$$

Here $\Pi^\mu=\partial^\mu\phi$, so $T^{\mu\nu}=\partial^\mu\phi\partial^\nu\phi-\eta^{\mu\nu}\mathcal L$. Raising the charge index gives the [four-momentum of a free real scalar field](../../../../../four-momentum-of-a-free-real-scalar-field.md),

$$
\boxed{E=P^0=\frac12\int d^3x\,\bigl(\dot\phi^2+|\nabla\phi|^2+m^2\phi^2\bigr),\qquad\mathbf P=-\int d^3x\,\dot\phi\,\nabla\phi.}
$$

The first is total [energy](../../../../../energy.md), and the three components of the second are physical spatial [momentum](../../../../../momentum.md). With signature $(+,-,-,-)$, $P_i=-P^i$; this explains the opposite sign if the conserved quantities are instead written with lower spatial indices. For example, a [plane wave](../../../../../plane-wave.md) proportional to $\cos(Et-\mathbf k\cdot\mathbf x)$ has [momentum](../../../../../momentum.md) density along $\mathbf k$, confirming the sign. All charges require convergence of the integrals and vanishing boundary flux, or periodic [boundary conditions](../../../../../boundary-condition.md) in a finite box.

For the [complex scalar field](../../../../../complex-scalar-field.md), treat $\psi$ and $\psi^*$ as independent variables when varying, equivalently use their two real components. The [global phase symmetry of a complex scalar field](../../../../../global-phase-symmetry-of-a-complex-scalar-field.md) is $\psi\mapsto e^{-i\alpha}\psi$, $\psi^*\mapsto e^{i\alpha}\psi^*$ for constant $\alpha$. Both the [kinetic term](../../../../../kinetic-term.md) and $V(|\psi|^2)$ are invariant. This is a global [internal symmetry of a classical field theory](../../../../../internal-symmetry-of-a-classical-field-theory.md) with [circle group](../../../../../circle-group.md) $U(1)$; a spacetime-dependent phase would require a gauge connection.

Choosing this orientation for the phase parameter gives the [Noether charge of a complex scalar field](../../../../../noether-charge-of-a-complex-scalar-field.md):

$$
\boxed{j^\mu=i\bigl(\psi^*\partial^\mu\psi-\psi\partial^\mu\psi^*\bigr),\qquad Q=i\int d^3x\,\bigl(\psi^*\dot\psi-\psi\dot\psi^*\bigr).}
$$

To check conservation directly, the [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md) are $\Box\psi+V'(|\psi|^2)\psi=0$ and their [complex conjugates](../../../../../complex-conjugate.md), assuming a real differentiable potential. Hence $\partial_\mu j^\mu=i(\psi^*\Box\psi-\psi\Box\psi^*)=0$. Reversing the phase-parameter orientation reverses the current and charge, which is merely a convention. **For a [scalar](../../../../../scalar.md) carrying [electric charge](../../../../../electric-charge.md) $q$, the physical [electric charge](../../../../../electric-charge.md) is $qQ$ after electromagnetic coupling.** In a neutral theory the same global charge can instead label an internal conserved [quantum number](../../../../../quantum-number.md); the density alone does not identify it automatically with electricity.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
