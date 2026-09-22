<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An ideal $\pi$ pulse is $-i\sigma_\phi$. Since $\sigma_\phi\sigma_{2\phi}\sigma_\phi=\sigma_x$, the chronological three-pulse sequence has propagator

$$
\boxed{R_\phi(\pi)R_{2\phi}(\pi)R_\phi(\pi)=i\sigma_x.}
$$

It implements the [Pauli X gate](../../../../pauli-x-gate.md) up to [global phase](../../../../global-phase.md), for every $\phi$.

For this [three-pulse amplitude-error compensation](../../../../three-pulse-amplitude-error-compensation.md), the leading error in the supplied fidelity expansion vanishes when $1+2\cos\phi=0$, giving

$$
\boxed{\phi=\frac{2\pi}{3}\quad\text{or}\quad\frac{4\pi}{3}\pmod{2\pi}.}
$$

These choices minimize the leading small-angle-error infidelity. Substituting $\cos\phi=\cos2\phi=-1/2$ into the fourth-order term gives

$$
\boxed{\mathcal F_3=1-\frac{3\pi^4}{128}\epsilon^4+O(\epsilon^6).}
$$

The fourth-order coefficient is nonzero, so this three-pulse sequence improves the single pulse's quadratic infidelity to quartic infidelity, rather than sixth-order infidelity.

An exact check is available. With $x=\pi\epsilon/2$, multiplication of the three imperfect [rotation gates](../../../../rotation-gate.md) at either optimum gives

$$
\boxed{\mathcal F_3=\left|\cos x\left(1+\frac12\sin^2x\right)\right|.}
$$

Its [Taylor expansion](../../../../taylor-expansion.md) has precisely the fourth-order coefficient above. The improvement concerns the same systematic fractional angle error on all three pulses; other errors need not cancel.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
