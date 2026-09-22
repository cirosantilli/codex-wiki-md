<h1 id="15a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the prepared [wavefunction](../../../../../../wave-function.md) real and positive on its support. Its normalization is

$$
\psi(x)=\frac{\sqrt3}{a^{3/2}}x\quad(0<x<a),\qquad \psi(x)=0\quad\text{elsewhere}.
$$

In the [ramp-state expansion in a symmetric infinite well](../../../../../../ramp-state-expansion-in-a-symmetric-infinite-well.md), write $\psi=\sum_{n\geq1}c_n\psi_n$. Orthogonality gives

$$
c_n=\frac{\sqrt3}{a^2}\int_0^a x\sin\left(\frac{n\pi(x+a)}{2a}\right)\,dx.
$$

For $\kappa=n\pi/(2a)$, a primitive is $-x\cos(\kappa(x+a))/\kappa+\sin(\kappa(x+a))/\kappa^2$. Evaluating both endpoints gives

$$
\boxed{c_n=-\frac{2\sqrt3(-1)^n}{n\pi}-\frac{4\sqrt3\sin(n\pi/2)}{n^2\pi^2}.}
$$

An equivalent parity-separated form is

$$
\boxed{c_{2p}=-\frac{\sqrt3}{p\pi},\qquad c_{2p-1}=\frac{2\sqrt3}{(2p-1)\pi}\left[1+\frac{2(-1)^p}{(2p-1)\pi}\right].}
$$

These formulas with $\sum_n c_n\psi_n$ are the requested explicit expansion. The convergence is in the square-integrable norm; at the idealized discontinuity at the right wall, a pointwise boundary value does not change the quantum state or its [probability amplitudes](../../../../../../probability-amplitude.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [15A](../../15a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
