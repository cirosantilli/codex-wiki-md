<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take $|L\rangle=|0\rangle$ and $|R\rangle=|1\rangle$. Initially the two masses are in the [product state](../../../../../product-state.md)

$$
|\psi(0)\rangle=\frac12(|LL\rangle+|LR\rangle+|RL\rangle+|RR\rangle).
$$

The branch-dependent [Newtonian gravitational potential energy](../../../../../newtonian-gravitational-potential-energy.md) is $-Gm^2/d_{ab}$. Under the stated approximation, only the $|RL\rangle$ branch acquires an appreciable relative phase, so after time $t$,

$$
|\psi(t)\rangle\simeq
\frac12(|LL\rangle+|LR\rangle+e^{i\phi}|RL\rangle+|RR\rangle),
\qquad
\phi=\frac{Gm^2t}{\hbar d}.
$$

The determinant of its two-by-two coefficient matrix is $(1-e^{i\phi})/4$, which is nonzero unless $\phi$ is a multiple of $2\pi$. Thus the state generally has [Schmidt rank](../../../../../schmidt-rank.md) two: the branch-dependent gravitational phase creates [gravitationally induced entanglement](../../../../../gravitationally-induced-entanglement.md).

An [entanglement witness](../../../../../entanglement-witness.md) has a bound obeyed by every [separable quantum state](../../../../../separable-quantum-state.md) and violated by at least one entangled state. For a product state with [Bloch vectors](../../../../../bloch-vector.md) $\mathbf r$ and $\mathbf s$,

$$
|\langle X\otimes Z+Y\otimes Y\rangle|
=|r_xs_z+r_ys_y|
\leq\sqrt{r_x^2+r_y^2}\sqrt{s_z^2+s_y^2}
\leq1
$$

by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). Convexity gives the same bound for every separable mixed state. Consequently $W>1$ certifies entanglement; in conventional operator form, one of $I\mp(X\otimes Z+Y\otimes Y)$ has negative expectation whenever the absolute-value criterion is violated.

For the state above, direct use of the [Pauli matrices](../../../../../pauli-matrices.md) gives

$$
\langle X\otimes Z\rangle
=\langle Y\otimes Y\rangle
=\frac{\cos\phi-1}{2},
\qquad
W=1-\cos\phi.
$$

With the supplied values,

$$
\phi\simeq
\frac{(6.674\times10^{-11})(10^{-14})^2(10)}
{(1.054\times10^{-34})(2\times10^{-4})}
\simeq3.17,
$$

which is close to $\pi$. Hence $W\simeq2.00$, and to the nearest integer

$$
\boxed{W=2}.
$$

This is the operating principle of the [Bose--Marletto--Vedral experiment](../../../../../bose-marletto-vedral-experiment.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 325](../../paper-325-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
