<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [variational symmetry of a Lagrangian density](../../../../variational-symmetry-of-a-lagrangian-density.md) maps admissible field configurations to configurations with the same [action](../../../../action.md), up to an allowed boundary contribution. Thus (i) the [action](../../../../action.md) is invariant for suitable [boundary conditions](../../../../boundary-condition.md), while (ii) the [Lagrangian density](../../../../lagrangian-density.md) need only change by a [total divergence](../../../../total-divergence.md), rather than be pointwise invariant. For an [internal symmetry of a classical field theory](../../../../internal-symmetry-of-a-classical-field-theory.md), the coordinates are fixed. A spacetime transformation also changes the integration measure and must be treated accordingly.

A [conserved current](../../../../conserved-current.md) satisfies $\partial_\mu j^\mu=0$ [on shell](../../../../on-shell.md). The [Noether charge](../../../../noether-charge.md) $Q=\int j^0\,d^3x$ then obeys $\dot Q=-\int_{\partial V}\mathbf j\cdot d\mathbf S$, so conservation of the integrated charge additionally requires vanishing net boundary flux.

For several real field components $q_A$ and a constant infinitesimal parameter, write $\delta q_A=\varepsilon X_A$ and $\delta\mathcal L=\varepsilon\partial_\mu K^\mu$. The [product rule](../../../../product-rule.md) gives

$$
\frac{\delta\mathcal L}{\varepsilon}=\sum_A\left(\frac{\partial\mathcal L}{\partial q_A}-\partial_\mu\frac{\partial\mathcal L}{\partial(\partial_\mu q_A)}\right)X_A+\partial_\mu\left(\sum_A\frac{\partial\mathcal L}{\partial(\partial_\mu q_A)}X_A\right).
$$

Subtract the specified divergence. The [Euler-Lagrange field equations](../../../../euler-lagrange-field-equation.md) make the first term vanish, proving the [Noether theorem](../../../../noether-theorem.md) with

$$
\boxed{j^\mu=\sum_A\frac{\partial\mathcal L}{\partial(\partial_\mu q_A)}X_A-K^\mu,\qquad \partial_\mu j^\mu=0.}
$$

For a [complex scalar field](../../../../complex-scalar-field.md), treat the field and its [complex conjugate](../../../../complex-conjugate.md) as independent variables in this calculation; this is equivalent to using its two real components. This is the [Noether current for a first-derivative scalar field](../../../../noether-current-for-a-first-derivative-scalar-field.md), summed over components.

Collect the two complex fields into $\Phi=(\phi_1,\phi_2)^T$. Their [Lagrangian density](../../../../lagrangian-density.md) has the radial form

$$
\mathcal L=\partial_\mu\Phi^\dagger\partial^\mu\Phi-m^2\Phi^\dagger\Phi-\lambda(\Phi^\dagger\Phi)^2.
$$

For a constant [Hermitian matrix](../../../../hermitian-operator.md) $T$, the [unitary transformation](../../../../unitary-operator.md) $\delta\Phi=i\varepsilon T\Phi$ preserves both the kinetic contraction and $\Phi^\dagger\Phi$. In particular the two specified transformations have generators $T_1=\sigma_1$ and $T_2=\sigma_2$, the first two [Pauli matrices](../../../../pauli-matrices.md). Their [Noether currents](../../../../noether-current.md) are instances of the [unitary scalar multiplet current](../../../../unitary-scalar-multiplet-current.md)

$$
j_T^\mu=i\left[(\partial^\mu\Phi^\dagger)T\Phi-\Phi^\dagger T\partial^\mu\Phi\right].
$$

Explicitly,

$$
\begin{aligned}
j_1^\mu&=i\left(\phi_2\partial^\mu\phi_1^*+\phi_1\partial^\mu\phi_2^*-\phi_2^*\partial^\mu\phi_1-\phi_1^*\partial^\mu\phi_2\right),\\
j_2^\mu&=\phi_2\partial^\mu\phi_1^*-\phi_1\partial^\mu\phi_2^*+\phi_2^*\partial^\mu\phi_1-\phi_1^*\partial^\mu\phi_2.
\end{aligned}
$$

An overall change of current sign corresponds to reversing the associated symmetry parameter; the signs here follow the two transformations as written.

The [matrix commutator](../../../../commutator.md) of their infinitesimal matrices is $[i\sigma_1,i\sigma_2]=-2i\sigma_3$. The antisymmetric difference of successive transformations therefore supplies a third symmetry, after a nonzero rescaling of its parameter:

$$
\delta\phi_1=i\zeta\phi_1,\qquad\delta\phi_2=-i\zeta\phi_2.
$$

Its current is

$$
\boxed{j_3^\mu=i\left(\phi_1\partial^\mu\phi_1^*-\phi_1^*\partial^\mu\phi_1-\phi_2\partial^\mu\phi_2^*+\phi_2^*\partial^\mu\phi_2\right).}
$$

The three [traceless matrices](../../../../traceless-matrix.md) $\sigma_a/2$ obey $[\sigma_a/2,\sigma_b/2]=i\epsilon_{abc}\sigma_c/2$. Their exponentials act as [SU(2)](../../../../su-2-group.md) on the complex doublet. This identifies both the [Lie algebra](../../../../lie-algebra-split.md) and the group acting on these fields: the central element $-I$ changes $\Phi$ and is not the identity transformation, so the doublet action is not an action of $SO(3)$ obtained by identifying $I$ with $-I$.

There is also a common [global phase symmetry of a complex scalar field](../../../../global-phase-symmetry-of-a-complex-scalar-field.md), $\Phi\mapsto e^{i\alpha}\Phi$, with current $j_I^\mu$. Together with [SU(2)](../../../../su-2-group.md) this gives $U(2)\simeq(SU(2)\times U(1))/\mathbb Z_2$ among complex-linear transformations. Independent constant phases of $\phi_1$ and $\phi_2$, and field interchange, are already contained in this group.

In fact this particular [scalar potential](../../../../scalar-potential.md) has a larger real internal symmetry. Write $\phi_1=(q_1+iq_2)/\sqrt2$ and $\phi_2=(q_3+iq_4)/\sqrt2$; then

$$
\mathcal L=\frac12\sum_{A=1}^4\partial_\mu q_A\partial^\mu q_A-\frac{m^2}{2}\sum_Aq_A^2-\frac\lambda4\left(\sum_Aq_A^2\right)^2.
$$

The [O(4) symmetry of a complex scalar doublet](../../../../o-4-symmetry-of-a-complex-scalar-doublet.md) includes transformations mixing $\Phi$ with $\Phi^*$, which need not be complex-linear. Its connected part has six rotation generators, so listing $U(2)$ alone would not exhaust the internal symmetries of the displayed isolated theory. Individual field conjugations are examples of its discrete transformations. Finally the spacetime-independent scalar coefficients and Lorentz contractions give [Poincaré symmetry](../../../../poincare-symmetry.md), and the real scalar action also permits spatial reflection and time reversal. These statements concern the action; a chosen vacuum or external [boundary conditions](../../../../boundary-condition.md) can preserve fewer symmetries. Special parameter choices can introduce additional symmetries, but are not required here.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the gauge field theory course of the University of Cambridge](../../../split.md)
5. [Gauge Field Theory course of the University of Cambridge](../../../../gauge-field-theory-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
