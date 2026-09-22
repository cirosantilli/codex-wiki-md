<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**True for the finite bound-level Morse model with nonzero adjacent control couplings.** The [Morse oscillator](../../../../../../morse-oscillator.md) energies have the form

$$
E_n=A(n+1/2)-B(n+1/2)^2,
\qquad E_{n+1}-E_n=A-2B(n+1).
$$

Over the physical bound-level range these adjacent gaps are positive, and $B\ne0$ makes them pairwise distinct. Label the retained levels consecutively. With $H_1=\sum_j d_j(E_{j,j+1}+E_{j+1,j})$, all $d_j\ne0$, the squared adjoint action of $iH_0$ has [eigenvalue](../../../../../../eigenvalue.md) $-(E_{j+1}-E_j)^2$ on each adjacent skew-Hermitian coupling. A polynomial chosen by [Lagrange interpolation](../../../../../../lagrange-polynomial.md) can therefore isolate any one adjacent coupling from $iH_1$.

Commuting an isolated coupling once with the drift produces its independent antisymmetric quadrature. The bracket between the two quadratures yields a traceless diagonal generator; brackets along the connected chain produce every nonadjacent off-diagonal generator. Thus [connected nondegenerate transition chain generates special unitary control](../../../../../../connected-nondegenerate-transition-chain-generates-special-unitary-control.md) proves $\mathfrak{su}(N)\subseteq\mathfrak g$, which gives density-state controllability. If the physical drift has nonzero [trace](../../../../../../matrix-trace.md), subtracting its traceless part also produces the identity direction, giving $\mathfrak u(N)$ and full operator controllability. Shifting the energy origin may remove that extra phase direction but does not change state controllability. The assertion concerns the finite-level model in the question, not the entire bound-plus-dissociation [Hilbert space](../../../../../../hilbert-space-split.md) of the untruncated Morse potential.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
