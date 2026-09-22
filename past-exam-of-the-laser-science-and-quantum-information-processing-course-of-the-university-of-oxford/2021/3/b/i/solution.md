<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the stated [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md), put $\boldsymbol\Omega=(V,0,-\delta)$ and $\Omega=\sqrt{V^2+\delta^2}$. The [Bloch vector](../../../../../bloch-vector.md) obeys

$$
\dot{\mathbf r}=\boldsymbol\Omega\mathbin\times\mathbf r,\qquad
U(t)=\cos\frac{\Omega t}{2}\,I-i\sin\frac{\Omega t}{2}\,
\frac{V\sigma_x-\delta\sigma_z}{\Omega}.
$$

Thus it rotates right-handedly about the fixed axis $\boldsymbol\Omega$, preserving its length and its projection on that axis. For example, on [resonance](../../../../../resonance.md) $\delta=0$, a north-pole [Bloch vector](../../../../../bloch-vector.md) follows $(0,-\sin Vt,\cos Vt)$ and reaches the south pole at $t=\pi/V$.

Take $V>0$, with the field [phase](../../../../../phase-waves.md) chosen accordingly. The [Hadamard gate](../../../../../hadamard-gate.md) is $H=(\sigma_x+\sigma_z)/\sqrt2$. Align the axis with $(1,0,1)$ and rotate through $\pi$:

$$
\boxed{\delta=-V,\qquad \tau=\frac{\pi}{\sqrt2V},\qquad U(\tau)=-iH.}
$$

The factor $-i$ is an irrelevant common [global phase](../../../../../global-phase.md). This realizes the whole [quantum gate](../../../../../quantum-logic-gate.md), rather than merely its action on one input [quantum state](../../../../../quantum-state.md).

There is a [basis](../../../../../basis.md)-ordering convention to make explicit: this $H$ is the [Hadamard gate](../../../../../hadamard-gate.md) matrix in the ordered [basis](../../../../../basis.md) $(|1\rangle,|0\rangle)$ chosen in part (a). If instead its definition is the usual ket rules $H_{01}|0\rangle=(|0\rangle+|1\rangle)/\sqrt2$ and $H_{01}|1\rangle=(|0\rangle-|1\rangle)/\sqrt2$, its matrix in our order is $(\sigma_x-\sigma_z)/\sqrt2$. For that definition choose $\boxed{\delta=+V,\ \tau=\pi/(\sqrt2V)}$. Both conventions use the same pulse duration; the sign of the [Rabi detuning](../../../../../rabi-detuning.md) selects the desired axis.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../../split.md)
6. [Laser science and quantum information processing course of the University of Oxford](../../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
7. [Year 4 of the physics course of the University of Oxford](../../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
