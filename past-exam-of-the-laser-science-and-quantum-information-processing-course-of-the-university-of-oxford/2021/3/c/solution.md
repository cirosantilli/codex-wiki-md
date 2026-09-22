<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep the [Pauli matrix](../../../../pauli-matrices.md) and north-pole conventions of part (a), and neglect [Rabi detuning](../../../../rabi-detuning.md) during each short pulse. Write $P=R_x(\pi/2)$ and $\phi=\delta T$. During the first pulse the [Bloch vector](../../../../bloch-vector.md) is $(0,-\sin\theta,\cos\theta)$ for $0\leq\theta\leq\pi/2$. During free evolution,

$$
\mathbf r(t)=(-\sin\delta t,-\cos\delta t,0),\qquad 0\leq t\leq T,
$$

because the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) generates $R_z(-\delta t)$. During the final pulse it is

$$
\mathbf r_{\rm last}(\theta)=(-\sin\phi,-\cos\phi\cos\theta,-\cos\phi\sin\theta),
\quad 0\leq\theta\leq\pi/2.
$$

These formulas specify every arc in the two [Bloch sphere](../../../../bloch-sphere.md) sketches. For $T=\pi/(2\delta)$ the path is north $\to-y\to-x$, and the last pulse leaves $-x$ fixed. For $T=\pi/\delta$ the path is north $\to-y\to+y\to$ north.

To test the complete [quantum gate](../../../../quantum-logic-gate.md), multiply its [unitary operators](../../../../unitary-operator.md):

$$
\begin{aligned}
U_R&=P e^{i\phi\sigma_z/2}P\\
&=-i\left[\cos(\phi/2)\sigma_x-\sin(\phi/2)\sigma_z\right].
\end{aligned}
$$

It is proportional to the [Hadamard gate](../../../../hadamard-gate.md) when $\cos(\phi/2)=-\sin(\phi/2)$, hence the shortest positive waiting time is

$$
\boxed{T_H=\frac{3\pi}{2\delta},\qquad U_R(T_H)=iH.}
$$

More generally $\delta T=-\pi/2\pmod{2\pi}$. With the alternative conventional ket definition $H_{01}$ specified in part (b)(i), the required matrix is $(\sigma_x-\sigma_z)/\sqrt2$, so $\boxed{T_{H_{01}}=\pi/(2\delta)}$ and $U_R=-iH_{01}$. The distinction concerns which [basis](../../../../basis.md) order defines the named [Hadamard gate](../../../../hadamard-gate.md); the evolution and the return population do not depend on that naming choice. Finally $r_z=-\cos\phi$, so the actual return population is

$$
\boxed{\rho_{11}(T)=\frac{1-\cos(\delta T)}2=\sin^2(\delta T/2).}
$$

**The printed plus sign is inconsistent with the two identical pulses.** At $T=0$, $U_R=P^2=-i\sigma_x$, so $|1\rangle$ becomes $|0\rangle$ and $\rho_{11}(0)=0$; the printed expression gives one. This counterexample is independent of [Bloch sphere](../../../../bloch-sphere.md) labeling. A plus sign would describe the complementary population $\rho_{00}$, or the return population with an opposite-sign final pulse. That changed sequence also changes the gate question and must not be silently substituted.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
