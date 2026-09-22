# Paper 325

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_325.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_325.pdf)

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
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let a [projective measurement](../../../quantum-measurement.md#projective-measurement) have mutually [orthogonal projections](../../../hilbert-space.md#orthogonal-projection) $P_i$ satisfying $\sum_iP_i=I$. On a [density operator](../../../quantum-theory.md#density-matrix) $\rho$, the [Born rule](../../../quantum-mechanics.md#born-rule) and the [Lüders rule](../../../quantum-measurement.md#luders-rule) give

$$
\Pr(i)=\operatorname{Tr}(P_i\rho),
\qquad
\rho\longmapsto
\frac{P_i\rho P_i}{\operatorname{Tr}(P_i\rho)}
$$

conditional on outcome $i$. On the first part of a [bipartite quantum system](../../../quantum-mechanics.md#tensor-product-of-quantum-systems), replace $P_i$ by $P_i\otimes I_2$.

The subsystems are isolated when there is no interaction term coupling them. Their [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) has the form

$$
H=H_1\otimes I_2+I_1\otimes H_2,
$$

so their subsequent [unitary time evolution](../../../quantum-mechanics.md#unitary-time-evolution) factorizes as $U_1\otimes U_2$.

The [reduced density matrix](../../../bell-state.md#reduced-density-matrix) of subsystem 1 is

$$
\boxed{\rho_1=\operatorname{Tr}_2\rho_{12}},
$$

where the [partial trace](../../../quantum-theory.md#partial-trace) is characterized by

$$
\operatorname{Tr}_1(M_1\rho_1)
=\operatorname{Tr}_{12}[(M_1\otimes I_2)\rho_{12}]
$$

for every local [observable](../../../quantum-mechanics.md#observable) $M_1$. Thus $\rho_1$ contains exactly the statistics accessible by measurements on subsystem 1.

Suppose a projective measurement $\{Q_j\}$ is performed on subsystem 2 and its outcome is not communicated. The resulting nonselective state is

$$
\rho'_{12}=\sum_j(I_1\otimes Q_j)\rho_{12}(I_1\otimes Q_j).
$$

For every $M_1$, the [cyclic property of the trace](../../../linear-algebra.md#cyclic-property-of-the-trace) and $\sum_jQ_j^2=I_2$ give

$$
\begin{aligned}
\operatorname{Tr}[(M_1\otimes I_2)\rho'_{12}]
&=\sum_j\operatorname{Tr}[(M_1\otimes Q_j^2)\rho_{12}]\\
&=\operatorname{Tr}[(M_1\otimes I_2)\rho_{12}].
\end{aligned}
$$

Hence $\rho'_1=\rho_1$. No local projective measurement on subsystem 1 can reveal whether the remote unreported measurement occurred. This is [quantum no-signalling](../../../quantum-theory.md#quantum-no-signalling), which prevents a choice made at a [spacelike separation](../../../special-relativity.md#spacelike-separation) from transmitting information faster than light and makes the measurement formalism compatible with [relativistic causality](../../../special-relativity.md#relativistic-causality).

The proposed nondisturbing device would violate [no information without disturbance](../../../quantum-measurement.md#no-information-without-disturbance). In an ordinary quantum instrument, let $M_{i\alpha}$ be the [Kraus operators](../../../quantum-information-theory.md#kraus-operator) associated with classical output $i$. If every pure state $|\psi\rangle$ remains unchanged even conditional on the displayed outcome, every nonzero $M_{i\alpha}|\psi\rangle$ must be parallel to $|\psi\rangle$. A linear operator for which every vector is an [eigenvector](../../../linear-operator-theory.md#eigenvector) is a scalar multiple of the identity, so $M_{i\alpha}=c_{i\alpha}I$. Its output probability

$$
\sum_\alpha\langle\psi|M_{i\alpha}^\dagger M_{i\alpha}|\psi\rangle
=\sum_\alpha|c_{i\alpha}|^2
$$

is independent of the state. It cannot equal $\langle\psi|P_i|\psi\rangle$ for arbitrary projectors. Equivalently, repeated nondisturbing samples would permit [quantum state tomography](../../../quantum-measurement.md#quantum-state-tomography) of one specimen and then [quantum cloning](../../../quantum-theory.md#quantum-cloning), contradicting ordinary quantum theory.

Such devices would not _necessarily_ enable [superluminal signalling](../../../special-relativity.md#faster-than-light-communication). One consistent operational extension could make every sequence of outputs depend only on the local [reduced density matrix](../../../bell-state.md#reduced-density-matrix) and local settings. Since an unreported remote measurement leaves that matrix unchanged, all local device statistics would remain unchanged too. Other extensions could add nonlocal outcome-dependent rules and permit signalling, but that behavior is additional to the device specification rather than forced by it.

## 2

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For the [spin singlet state](../../../bell-state.md#spin-singlet-state), measurements along the same axis are perfectly anticorrelated. By measuring either spin component of particle $B$, one can therefore predict with certainty the corresponding result for distant particle $A$. The [Einstein–Podolsky–Rosen criterion of reality](../../../quantum-theory.md#einstein-podolsky-rosen-criterion-of-reality) then says that every such spin component of $A$ is an element of physical reality, because the choice at $B$ can be made without disturbing $A$. Since the quantum state assigns no simultaneous sharp values to noncommuting spin components, the EPR argument concludes that the wavefunction is not a complete description, provided this locality premise is accepted.

Let $\lambda$ denote a proposed complete hidden state, and let $a,b$ be the chosen axes.

- [Outcome determinism](../../../quantum-theory.md#outcome-determinism) says that, given $\lambda$ and the settings, each outcome is fixed rather than merely probabilistic: $A,B\in\{-1,1\}$ are definite response functions.
- [Parameter independence](../../../quantum-theory.md#parameter-independence) says that the conditional distribution of one local outcome is independent of the distant setting. Together with outcome determinism, it gives $A=A(a,\lambda)$ and $B=B(b,\lambda)$.
- [Measurement independence](../../../quantum-theory.md#measurement-independence) says that the preparation variable is statistically independent of the later settings: $\rho(\lambda|a,b)=\rho(\lambda)$.

For two axes on each side, every $\lambda$ obeys

$$
\begin{aligned}
S(\lambda)
&=A(a_0,\lambda)[B(b_0,\lambda)+B(b_1,\lambda)]\\
&\quad+A(a_1,\lambda)[B(b_0,\lambda)-B(b_1,\lambda)]
\in\{-2,2\}.
\end{aligned}
$$

[Measurement independence](../../../quantum-theory.md#measurement-independence) permits averaging the same distribution of $\lambda$ for all four setting pairs, producing the [CHSH inequality](../../../quantum-theory.md#chsh-inequality)

$$
|E_{00}+E_{01}+E_{10}-E_{11}|\leq2.
$$

The singlet prediction is

$$
E(a,b)=-\mathbf a\mathbin\cdot\mathbf b.
$$

Choose coplanar unit vectors

$$
\mathbf a_0=\mathbf z,
\qquad
\mathbf a_1=\mathbf x,
\qquad
\mathbf b_0=\frac{\mathbf z+\mathbf x}{\sqrt2},
\qquad
\mathbf b_1=\frac{\mathbf z-\mathbf x}{\sqrt2}.
$$

Then

$$
E_{00}=E_{01}=E_{10}=-\frac1{\sqrt2},
\qquad
E_{11}=\frac1{\sqrt2},
$$

and therefore

$$
\boxed{|E_{00}+E_{01}+E_{10}-E_{11}|=2\sqrt2>2}.
$$

Thus the predictions of quantum theory violate the conjunction of outcome determinism, parameter independence, and measurement independence. This is [Bell theorem](../../../quantum-theory.md#bell-theorem); the calculation alone does not select which premise a deeper theory must abandon.

## 3

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

In the [Page–Geilker experiment](../../../quantum-theory.md#page-geilker-experiment), radioactive-decay counts supplied a quantum random decision that determined which of two macroscopically distinct configurations of lead masses the experimenters placed around a [Cavendish torsion balance](../../../classical-mechanics.md#cavendish-torsion-balance). In each observed branch, the balance deflected in the direction predicted by the mass configuration recorded in that branch, with a strong correlation between the decision and the measured gravitational torque.

The unobserved alternative was the prediction of the simplest [semiclassical Einstein equation](../../../quantum-theory.md#semiclassical-einstein-equation), in which one classical metric is sourced by the expectation value $\langle T_{\mu\nu}\rangle$ of the matter [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor). If the universal wavefunction does not collapse, the two nearly equally weighted mass configurations both contribute to that expectation value. Their opposite torques should then largely average away, and the balance should show little branch-correlated deflection. That behavior was not seen.

The experiment was designed to go beyond earlier observations of ordinary gravity and quantum matter. It deliberately created macroscopically different mass distributions in different quantum branches and tested whether the gravitational field followed the branch actually observed or the expectation-value average over all branches. It ruled out that simplest no-collapse semiclassical coupling under the experiment's assumptions. It supplied indirect evidence for [quantum gravity](../../../quantum-theory.md#quantum-gravity), while leaving more elaborate classical-quantum couplings logically possible.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a neutron in the Earth's [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential) $\Phi_E$, the [Schrödinger equation](../../../physics.md#schrodinger-equation) is

$$
\boxed{
i\hbar\frac{\partial\psi}{\partial t}
=\left[-\frac{\hbar^2}{2m_n}\nabla^2+m_n\Phi_E\right]\psi}.
$$

Near the surface, $\Phi_E(z)=gz$ up to an additive constant.

The [Colella–Overhauser–Werner experiment](../../../quantum-mechanics.md#colella-overhauser-werner-experiment) uses crystal slabs as coherent beam splitters and mirrors in a [neutron interferometer](../../../quantum-mechanics.md#neutron-interferometer). The two paths contain horizontal segments of length $s$ separated vertically by $r$, then recombine. The [gravitational potential energy](../../../classical-mechanics.md#newtonian-gravitational-potential-energy) difference is $m_ngr$. A neutron of speed $v$ spends time $s/v$ on a horizontal segment, so the gravitationally induced relative [quantum phase](../../../quantum-mechanics.md#quantum-phase) is

$$
|\Delta\phi|
=\frac{m_ngr}{\hbar}\frac{s}{v}.
$$

Using the [de Broglie wavelength](../../../quantum-mechanics.md#de-broglie-wavelength) $\lambda=h/(m_nv)$ and $\hbar=h/(2\pi)$ gives

$$
\boxed{|\Delta\phi|
=\frac{2\pi m_n^2grs\lambda}{h^2}}.
$$

Rotating the apparatus changes the vertical projection of its enclosed area from zero to $rs$. The number of full interference oscillations is therefore

$$
N=\frac{|\Delta\phi_{\max}|}{2\pi}
=\frac{m_n^2grs\lambda}{h^2}.
$$

Here $rs=(\sqrt{10}\,\mathrm{cm})^2=10^{-3}\,\mathrm{m}^2$, so

$$
N=\frac{(1.67\times10^{-27})^2(9.8)(10^{-3})(1.42\times10^{-10})}
{(6.6\times10^{-34})^2}
\simeq8.9.
$$

The expected change is therefore $\boxed{9}$ oscillations to the nearest integer.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

**Yes in both directions.** The [Page–Geilker experiment](../../../quantum-theory.md#page-geilker-experiment) tests whether a classical gravitational field is sourced by the expectation value of macroscopically superposed matter configurations. The [Colella–Overhauser–Werner experiment](../../../quantum-mechanics.md#colella-overhauser-werner-experiment) uses the Earth's effectively classical field as an external potential and therefore does not distinguish an expectation-value semiclassical source law from a quantized gravitational field.

Conversely, the Colella–Overhauser–Werner experiment directly observes coherent [matter-wave interference](../../../quantum-mechanics.md#matter-wave-interference) and a gravitationally generated relative phase in a neutron wavefunction. Page and Geilker did not maintain and recombine coherent branches of the macroscopic source, and their torsion-balance measurement was not an interference experiment. Thus their experiment did not test the neutron gravitational phase effect. The experiments probe opposite sides of the coupling: quantum matter responding coherently to gravity, and gravity responding to branch-dependent quantum matter.

## 4

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For particle positions $\mathbf r_1,\mathbf r_2$, the two-particle [Schrödinger equation](../../../physics.md#schrodinger-equation) is

$$
\boxed{
i\hbar\frac{\partial\Psi}{\partial t}
=\left[-\frac{\hbar^2}{2m_1}\nabla_1^2
-\frac{\hbar^2}{2m_2}\nabla_2^2
-\frac{Gm_1m_2}{|\mathbf r_1-\mathbf r_2|}\right]\Psi}.
$$

Write $|a\rangle_i$ for the localized [wave packet](../../../wave-equation.md#wave-packet) $\psi_{ai}$ and $d_{ab}=|x_{a1}-x_{b2}|$. Neglecting packet spreading and branch overlap, the initial [product state](../../../bell-state.md#product-state) evolves branchwise as

$$
|\Psi(t)\rangle\simeq\frac12\sum_{a,b=0}^1
\exp\left(\frac{iGm_1m_2t}{\hbar d_{ab}}\right)
|a\rangle_1|b\rangle_2,
$$

up to phases generated independently on the two particles. These branch-dependent phases generally cannot be separated into one phase depending only on $a$ and one depending only on $b$, so the [Newtonian gravitational potential energy](../../../classical-mechanics.md#newtonian-gravitational-potential-energy) creates [gravitationally induced entanglement](../../../quantum-theory.md#gravitationally-induced-entanglement).

If $d_{10}=|x_{11}-x_{02}|=d$ is much smaller than the other separations, remove their nearly common phase and retain only

$$
\phi=\frac{Gm_1m_2t}{\hbar d}.
$$

The state is approximately

$$
|\Psi(t)\rangle
=\frac12\left(|00\rangle+|01\rangle
+e^{i\phi}|10\rangle+|11\rangle\right).
$$

Its [concurrence](../../../bell-state.md#concurrence) is $|\sin(\phi/2)|$, so it becomes [maximally entangled](../../../quantum-theory.md#maximally-entangled-state) first at $\phi=\pi$. For $m_1=m_2=m$,

$$
\boxed{t_{\rm ent}
=\frac{\pi\hbar d}{Gm^2}
=\frac{hd}{2Gm^2}}
=\frac{(6.6\times10^{-34})(2\times10^{-4})}
{2(6.7\times10^{-11})(10^{-14})^2}
\simeq9.9\ \mathrm{s}.
$$

Thus the near-maximal entanglement time is about $\boxed{10\ \mathrm{s}}$ within the stated approximation.

A single prescribed [classical gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential) gives a Hamiltonian of the form $H_1[\Phi]\otimes I+I\otimes H_2[\Phi]$. Its evolution factorizes as $U_1\otimes U_2$ and preserves every initial [product state](../../../bell-state.md#product-state), so it cannot generate this entanglement. A semiclassical mean field sourced only by expectation values likewise gives each particle a local one-body potential and does not provide a quantum mediator carrying branch correlations.

An [entanglement witness](../../../quantum-information-theory.md#entanglement-witness) is a [Hermitian operator](../../../hilbert-space.md#hermitian-operator) $W$ whose expectation is nonnegative on every [separable state](../../../quantum-information-theory.md#separable-quantum-state) but negative on at least one [entangled state](../../../bell-state.md#entangled-state). At $\phi=\pi$, define

$$
|\Psi_*\rangle
=\frac12(|00\rangle+|01\rangle-|10\rangle+|11\rangle),
\qquad
W=\frac12I-|\Psi_*\rangle\langle\Psi_*|.
$$

The largest [Schmidt coefficient](../../../von-neumann-entropy.md#schmidt-coefficient) of $|\Psi_*\rangle$ is $1/\sqrt2$, so every product state $|u\rangle|v\rangle$ in the four-dimensional branch subspace satisfies $|\langle\Psi_*|u,v\rangle|^2\leq1/2$. By closure under [convex combinations](../../../mathematical-optimization.md#convex-combination), $\operatorname{Tr}(W\rho_{\rm sep})\geq0$ for every separable mixture, whereas

$$
\langle\Psi_*|W|\Psi_*\rangle=-\frac12.
$$

A negative measured value therefore certifies entanglement. Under the assumptions that the masses began unentangled and interacted only through gravity, such certification would show that the mediator can transmit quantum coherence; it would be evidence against a purely classical gravitational channel and for the quantum nature of gravity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
