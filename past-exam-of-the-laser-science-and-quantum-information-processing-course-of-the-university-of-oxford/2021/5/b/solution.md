<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On Bob's polarization [qubit](../../../../qubit.md), take

$$
X=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad
Z=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad
XZ=\begin{pmatrix}0&-1\\1&0\end{pmatrix}=-iY.
$$

Suitable conditional [unitary operators](../../../../unitary-operator.md) are

$$
\boxed{U_{\Phi^+}=XZ,\quad U_{\Phi^-}=X,\quad
U_{\Psi^+}=Z,\quad U_{\Psi^-}=I.}
$$

Indeed $(I\otimes XZ)|\Phi^+\rangle=|\Psi^-\rangle$, $(I\otimes X)|\Phi^-\rangle=|\Psi^-\rangle$, and $(I\otimes Z)|\Psi^+\rangle=-|\Psi^-\rangle$. The last minus sign is a harmless [global phase](../../../../global-phase.md).

For an ideal [half-wave plate](../../../../half-wave-plate.md) whose fast axis makes [angle](../../../../angle.md) $\theta$ with horizontal polarization, discard the common [phase](../../../../phase-waves.md) and use the [Jones matrix](../../../../jones-matrix.md)

$$
W(\theta)=\begin{pmatrix}\cos2\theta&\sin2\theta\\\sin2\theta&-\cos2\theta\end{pmatrix}.
$$

It implements $Z$ at $0^\circ$ and $X$ at $45^\circ$. Thus for outcome $\Phi^+$ use two [half-wave plates](../../../../half-wave-plate.md), first $0^\circ$ then $45^\circ$ in the propagation direction; for $\Phi^-$ use one at $45^\circ$; for $\Psi^+$ one at $0^\circ$; for $\Psi^-$ use no plate. Ideal retardance is assumed at the [photon](../../../../photon.md) [wavelength](../../../../wavelength.md), and the setting is chosen after receiving the detector's classical result.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
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
