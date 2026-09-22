<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

From [b](../b.md), the excited-state [probability](../../../../probability.md) is

$$
\boxed{P_e(t)=\cos^2(gt).}
$$

For a single short [measurement](../../../../quantum-measurement-split.md) interval $\Delta t$ beginning in $|e,0\rangle$, requiring $P_e>0.9$ before the first departure from unity gives

$$
\boxed{\Delta t<\frac{\arccos\sqrt{0.9}}g
=\frac{0.32175\ldots}{g}.}
$$

A zero-photon outcome resets the conditional state to $|e,0\rangle$. After $n=T/\Delta t$ such tests, the [probability](../../../../probability.md) of the all-zero-photon record is

$$
P_{\rm surv}(T)=[\cos^2(g\Delta t)]^n
\simeq e^{-g^2T\Delta t}.
$$

Thus a 90 percent survival requirement over a specified total duration $T$ is stronger than the single-interval condition: approximately $\Delta t<-\ln(0.9)/(g^2T)$ in the short-interval limit. The limiting preservation as $\Delta t\to0$ is the [quantum Zeno effect](../../../../quantum-zeno-effect.md).

The [measurement](../../../../quantum-measurement-split.md) instrument matters. If [photons](../../../../photon.md) are absorbed and their first detection removes the excitation, this survival [probability](../../../../probability.md) also equals the unconditional excited population. For ideal nondestructive [photon-number](../../../../photon-number.md) [measurements](../../../../quantum-measurement-split.md), excitation can transfer back after a one-photon result; the unconditional result after $n$ equal intervals is instead $P_e^{(n)}=[1+\cos^n(2g\Delta t)]/2$. It also tends to one for fixed $T$ as the intervals shrink. Neither interpretation guarantees indefinite 90 percent survival merely by imposing a 90 percent bound on each separate interval.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
