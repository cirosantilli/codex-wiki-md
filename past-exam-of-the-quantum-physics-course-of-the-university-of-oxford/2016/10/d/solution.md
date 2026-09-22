<h1 id="10/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Differentiate $\dot c_2=-i\gamma e^{2i\Omega t}c_1$ and substitute the equation for $\dot c_1$. The result is

$$
\boxed{\ddot c_2-2i\Omega\dot c_2+\gamma^2c_2=0.}
$$

Putting $c_2=e^{i\Omega t}u$ removes the first [derivative](../../../../derivative.md) and gives $\ddot u+\kappa^2u=0$, where $\kappa=\sqrt{\Omega^2+\gamma^2}$. For $\kappa>0$ the general solution is

$$
c_2=e^{i\Omega t}(A\cos\kappa t+B\sin\kappa t).
$$

The initial [spinor](../../../../spinor.md) fixes $c_1(0)=1,c_2(0)=0$, and the **first-order coupled equation** fixes the second initial datum $\dot c_2(0)=-i\gamma$. Thus $A=0$, $B=-i\gamma/\kappa$, and

$$
\boxed{c_2(t)=-i\frac\gamma\kappa e^{i\Omega t}\sin\kappa t,\qquad c_1(t)=e^{-i\Omega t}\left(\cos\kappa t+i\frac\Omega\kappa\sin\kappa t\right).}
$$

Their squared magnitudes sum to one. If both $\Omega$ and $\gamma$ vanish, the initial amplitudes simply remain $(1,0)$; the formulas have that continuous limit.

**Source convention correction.** For positive $\gamma$, the printed expression for $c_2$ lacks the factor $-i$ required by the stated [basis](../../../../basis.md) and initial [vector](../../../../vector.md). A concrete test is its [derivative](../../../../derivative.md) at $t=0$: the printed expression gives $+\gamma$, whereas the [Schrödinger equation](../../../../schrodinger-equation.md) gives $-i\gamma$. Multiplying only $c_2$ by a [phase](../../../../phase-waves.md) changes the relative [quantum phase](../../../../quantum-phase.md). One may change the overall [phase](../../../../phase-waves.md) of the entire [spinor](../../../../spinor.md), but must then transform $c_1$ and its initial amplitude as well. The printed modulus nevertheless gives the correct [transition probability](../../../../transition-probability.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [10](../../10.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum physics course of the University of Oxford](../../../split.md)
5. [Quantum physics course of the University of Oxford](../../../../quantum-physics-course-of-the-university-of-oxford.md)
6. [Year 2 of the physics course of the University of Oxford](../../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
