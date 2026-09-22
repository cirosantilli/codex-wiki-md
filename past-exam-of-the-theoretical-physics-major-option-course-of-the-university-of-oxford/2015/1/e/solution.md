<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For equal rates, the [master equation](../../../../master-equation.md) generator is $f$ times the symmetric path-graph matrix

$$
W/f=\begin{pmatrix}-1&1&0\\1&-2&1\\0&1&-1\end{pmatrix}.
$$

Its [eigenvectors](../../../../eigenvector.md) may be chosen as $(1,1,1)$, $(1,0,-1)$, and $(1,-2,1)$, with [eigenvalues](../../../../eigenvalue.md) $0,-f,-3f$. Resolve the initial empty state as

$$
(1,0,0)=\tfrac13(1,1,1)+\tfrac12(1,0,-1)+\tfrac16(1,-2,1).
$$

Each nonstationary eigencomponent decays with its own rate, giving

$$
\boxed{p_B(t)=\frac13-\frac12e^{-ft}+\frac16e^{-3ft}.}
$$

The remaining [probabilities](../../../../probability.md) are $p_0(t)=1/3+e^{-ft}/2+e^{-3ft}/6$ and $p_A(t)=(1-e^{-3ft})/3$. These satisfy the full equations and sum to one. The limit $p_B(\infty)=1/3$ agrees with the stationary result. At short times $p_B(t)=f^2t^2/2+O(t^3)$: two successive jumps, $0\to A\to B$, are necessary, so a term linear in $t$ would signal an incorrectly included direct transition.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
