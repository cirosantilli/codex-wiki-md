<h1 id="15b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [bound state](../../../../../../bound-state.md), $0<E<U_0$: the [Hamiltonian operator](../../../../../../hamiltonian-quantum-mechanics.md) is nonnegative, and an energy at or above the exterior potential does not give a nonzero [normalizable wavefunction](../../../../../../normalizable-wavefunction.md). The [Time-independent Schrödinger equation](../../../../../../time-independent-schrodinger-equation.md) and the hard wall at zero therefore give

$$
\psi(x)=A\sin(kx)\quad(0<x<a),\qquad \psi(x)=B e^{-\kappa(x-a)}\quad(x>a),
\qquad k=\frac{\sqrt{2mE}}{\hbar},\quad \kappa=\frac{\sqrt{2m(U_0-E)}}{\hbar}.
$$

Continuity of the [wavefunction](../../../../../../wave-function.md) and its derivative at the finite step gives $k\cot(ka)=-\kappa$. Put $z=ka$ and $z_0=a\sqrt{2mU_0}/\hbar$. The matching equation becomes

$$
z\cot z=-\sqrt{z_0^2-z^2},\qquad 0<z<z_0.
$$

It requires $\cot z<0$, so solutions lie in the intervals $((j+1/2)\pi,(j+1)\pi)$ for $j=0,1,\ldots$. Squaring, with that sign restriction retained, gives $z_0=z/|\sin z|$. On each such interval this function increases strictly from $(j+1/2)\pi$ to infinity: its derivative is $(|\sin z|-z\,\operatorname{sgn}(\sin z)\cos z)/\sin^2z>0$, because the second term in the numerator is positive there. Each interval therefore contributes exactly one [bound state](../../../../../../bound-state.md) if and only if $z_0>(j+1/2)\pi$. These are the [bound-state thresholds for a square well with one hard wall](../../../../../../bound-state-thresholds-for-a-square-well-with-one-hard-wall.md).

**Exactly one normalizable bound state exists if and only if**

$$
\boxed{\frac{\pi^2\hbar^2}{8ma^2}<U_0\leq\frac{9\pi^2\hbar^2}{8ma^2}.}
$$

**The printed strict upper inequality misses the threshold case.** At the upper endpoint, the prospective second state has $E=U_0$ and $\kappa=0$. Its exterior solution is constant or linear, hence is not square-integrable unless zero; the zero exterior solution and matching would force the entire solution to vanish. Thus there is still exactly one [bound state](../../../../../../bound-state.md) at that endpoint. The strict upper inequality is valid if threshold values are additionally excluded, but that exclusion is not part of the stated assumptions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15B](../../15b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
