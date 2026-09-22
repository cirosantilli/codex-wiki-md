<h1 id="section-b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use zero-based labels to agree with $\phi_0$ in the later parts. The normalized [infinite square well](../../../../../infinite-square-well.md) [energy eigenstates](../../../../../energy-eigenstate.md) and [energy eigenvalues](../../../../../energy-eigenvalue-split.md) are

$$
\phi_n(x)=\frac1{\sqrt a}\sin\left[\frac{(n+1)\pi(x+a)}{2a}\right],
\qquad \epsilon_n^{(0)}=K(n+1)^2,\quad
K=\frac{\pi^2\hbar^2}{8ma^2},\quad n=0,1,\ldots.
$$

The [position matrix elements in a symmetric infinite square well](../../../../../position-matrix-elements-in-a-symmetric-infinite-square-well.md), obtained by integrating the product of the two [wavefunctions](../../../../../wave-function-split.md) against $x$, are

$$
x_{kn}=\langle\phi_k|x|\phi_n\rangle
=\frac{8a(k+1)(n+1)[(-1)^{k+n}-1]}
{\pi^2[(k+1)^2-(n+1)^2]^2}\quad(k\ne n),\qquad x_{nn}=0.
$$

The integral in the question uses positive integer labels; replacing them by $k+1,n+1$ is essential here. Only opposite-parity states, $k+n$ odd, contribute, as also follows from the [parity operator](../../../../../parity-operator.md) [selection rule](../../../../../selection-rule.md).

[Second-order nondegenerate perturbation theory](../../../../../second-order-nondegenerate-perturbation-theory.md) now gives the requested infinite sum:

$$
\boxed{\delta\epsilon_n^{(2)}=e^2E^2\sum_{k\ne n}
\frac{|x_{kn}|^2}{\epsilon_n^{(0)}-\epsilon_k^{(0)}}.}
$$

In fully explicit form this is

$$
\boxed{\delta\epsilon_n^{(2)}=
-\frac{2048me^2E^2a^4}{\pi^6\hbar^2}(n+1)^2
\sum_{\substack{k\geq0\\k+n\ \mathrm{odd}}}
\frac{(k+1)^2}{[(k+1)^2-(n+1)^2]^5}.}
$$

The symbol $m$ here denotes the electron mass, not a summation index. For the [ground state](../../../../../ground-state.md) $n=0$, every denominator in the first form is negative, so the ground [energy level](../../../../../energy-level.md) moves downward. For excited states, contributions from lower and higher [energy levels](../../../../../energy-level.md) have opposite signs.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
