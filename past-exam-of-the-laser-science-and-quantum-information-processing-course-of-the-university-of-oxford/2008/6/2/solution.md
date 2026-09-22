<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Set $\omega_1=\omega_2=\omega$. Define the [quantum rotating frame](../../../../quantum-rotating-frame.md) by

$$
H_Z=\frac{\omega}{2}(Z\otimes I+I\otimes Z),\qquad
R(t)=e^{-itH_Z},\qquad
|\psi_{\mathrm r}(t)\rangle=R(t)^\dagger|\psi(t)\rangle.
$$

The isotropic [Heisenberg model](../../../../heisenberg-model.md) coupling commutes with the total $z$ [spin angular momentum](../../../../spin.md), so $[H_Z,C]=0$. The transformed [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) is therefore

$$
H_{\mathrm r}=R^\dagger H_{\mathrm H}R-iR^\dagger\dot R
=R^\dagger H_{\mathrm H}R-H_Z=\frac J2C.
$$

Here removal of the common [Zeeman energy](../../../../zeeman-energy.md) is exact; the exchange is resonant and cannot be discarded using the [weak coupling condition for two NMR spins](../../../../weak-coupling-condition-for-two-nmr-spins.md).

Put $a=Jt$, $c=\cos a$, and $s=\sin a$. Exponentiating the parallel-spin entries and the middle $2\times2$ [matrix](../../../../matrix.md) gives the [time-evolution operator](../../../../time-evolution-operator.md)

$$
\boxed{U(t)=e^{-itH_{\mathrm r}}=
\begin{pmatrix}
e^{-ia/2}&0&0&0\\
0&e^{ia/2}c&-ie^{ia/2}s&0\\
0&-ie^{ia/2}s&e^{ia/2}c&0\\
0&0&0&e^{-ia/2}
\end{pmatrix}.}
$$

For example, at $a=\pi/2$ this equals the [SWAP gate](../../../../swap-gate.md) times $e^{-i\pi/4}$, which checks both the exchange angle and the overall phase.

The printed network reads from left to right as $U$, a [Pauli Z gate](../../../../pauli-z-gate.md) on the **upper spin only**, $U$, and another upper-spin [Pauli Z gate](../../../../pauli-z-gate.md). Let

$$
P=Z\otimes I=\operatorname{diag}(1,1,-1,-1).
$$

Its total [time-evolution operator](../../../../time-evolution-operator.md), with the first operation on the right, is $W=PUPU$. For this [Heisenberg exchange echo](../../../../heisenberg-exchange-echo.md),

$$
PH_{\mathrm r}P=\frac J2(-X\otimes X-Y\otimes Y+Z\otimes Z).
$$

The three paired [Pauli operators](../../../../pauli-operator.md) $X\otimes X$, $Y\otimes Y$, $Z\otimes Z$ commute pairwise: for example both products $(X\otimes X)(Y\otimes Y)$ and $(Y\otimes Y)(X\otimes X)$ equal $-Z\otimes Z$. Thus $PH_{\mathrm r}P$ commutes with $H_{\mathrm r}$, and

$$
\boxed{W=e^{-itPH_{\mathrm r}P}e^{-itH_{\mathrm r}}
=e^{-iJtZ\otimes Z}
=\begin{pmatrix}
e^{-ia}&0&0&0\\
0&e^{ia}&0&0\\
0&0&e^{ia}&0\\
0&0&0&e^{-ia}
\end{pmatrix}.}
$$

The [spin echo](../../../../spin-echo.md) cancels the $XX+YY$ exchange terms and retains the [Ising coupling](../../../../ising-coupling-of-two-qubits.md). Equivalently, over the total free-evolution time $2t$ it produces the effective [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) $JZ\otimes Z/2$ exactly for ideal instantaneous gates. It is generally **not the identity**. A physical $\pi$ rotation about $z$ is $e^{-i\pi Z/2}=-iZ$; using two such pulses instead of the ideal $Z$ gates changes $W$ only by a physically irrelevant [global phase](../../../../global-phase.md) of minus one.

The implementation requires [frequency-selective spin control](../../../../frequency-selective-spin-control.md). Under the usual common-[radio frequency](../../../../radio-frequency.md) [NMR](../../../../nuclear-magnetic-resonance-split.md) assumptions, equal resonance frequencies give no way to apply a pulse to the first spin while leaving the second untouched. For equally coupled spins in a spatially uniform control field, the transverse control [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) has the form

$$
H_c(t)=\frac{u_x(t)}2(X\otimes I+I\otimes X)
+\frac{u_y(t)}2(Y\otimes I+I\otimes Y).
$$

Both this control and the drift [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) commute with the [SWAP gate](../../../../swap-gate.md) $S$. Every reachable [time-evolution operator](../../../../time-evolution-operator.md) consequently commutes with $S$. But $SPS=I\otimes Z\ne P$: the individual pulse required by the diagram fails this symmetry test. This is the [exchange symmetry obstruction to individual spin control](../../../../exchange-symmetry-obstruction-to-individual-spin-control.md). Applying simultaneous $Z$ gates gives $Q=Z\otimes Z$, which commutes with $H_{\mathrm r}$ and instead yields $QUQU=U^2$; it does not refocus the exchange. A common change of the RF phase reference also supplies only a collective rotation.

This obstruction assumes the usual common-RF control with no extra handle distinguishing the spins. Equal resonance frequencies do not universally forbid individual addressing: a spatially selective field, unequal control couplings, or another symmetry-breaking interaction could alter [controllability](../../../../controllability.md). Such resources are absent from the specified equivalent-spin [NMR](../../../../nuclear-magnetic-resonance-split.md) model.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [6](../../6-split.md)
3. [2008](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
