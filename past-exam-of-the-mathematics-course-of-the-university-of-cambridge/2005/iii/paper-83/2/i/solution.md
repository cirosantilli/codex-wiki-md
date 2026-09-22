<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The single-particle [Hamiltonian](../../../../../../hamiltonian.md) $H_0=-\hbar^2\partial_x^2/(2m)+V(x)$ has a [periodic potential](../../../../../../periodic-potential.md) $V(x+d)=V(x)$. Define the unitary [spatial translation operator](../../../../../../spatial-translation-operator.md) $T_d f(x)=f(x+d)$. Its derivatives commute with translation, and the potential's periodicity gives $H_0T_d=T_dH_0$.

Each energy eigenspace is therefore preserved by $T_d$, so within it one may choose simultaneous energy and translation eigenstates. On a large periodic interval of $M$ cells, $T_d^M=1$ and its eigenvalues are phases $\lambda=e^{ikd}$, with $k=2\pi j/(Md)$; the infinite-volume limit gives continuous quasimomentum modulo $2\pi/d$. For a simultaneous state in band $j$, this proves

$$
\boxed{\psi_{jk}(x+d)=e^{ikd}\psi_{jk}(x).}
$$

Then $u_{jk}(x)=e^{-ikx}\psi_{jk}(x)$ obeys $u_{jk}(x+d)=u_{jk}(x)$, which constructs the usual [Bloch state](../../../../../../bloch-state.md) rather than assuming its form. The label $j$ distinguishes [energy bands](../../../../../../energy-band.md) at the same [crystal momentum](../../../../../../crystal-momentum.md) $\hbar k$. In a degenerate energy eigenspace an arbitrary superposition need not itself have one translation phase; the result refers to the simultaneous [Bloch states](../../../../../../bloch-state.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
