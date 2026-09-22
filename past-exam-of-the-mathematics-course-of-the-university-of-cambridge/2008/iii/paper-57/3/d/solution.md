<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Replace the two arms by three identical arms of length $N$ attached to one central [qubit](../../../../../../qubit.md). Label the hub $c$ and the sites on arm $a$ by $(a,j)$, $a=1,2,3$, $j=1,\ldots,N$. Use [XY exchange interactions](../../../../../../xy-exchange-interaction.md) with coupling $J_0/\sqrt3$ on each hub-to-first-site link, and coupling $J_j$ on each arm link $(a,j)$ to $(a,j+1)$. Initially excite only the hub: this is the [product state](../../../../../../product-state.md) $|1\rangle_c$ with every arm [qubit](../../../../../../qubit.md) in $|0\rangle$.

In the symmetric [single-excitation subspace](../../../../../../single-excitation-subspace.md), define $|s_0\rangle=|c\rangle$ and $|s_j\rangle=3^{-1/2}\sum_{a=1}^3|a,j\rangle$. The hub coupling is

$$
H|s_0\rangle=\frac{J_0}{\sqrt3}\sum_{a=1}^3|a,1\rangle=J_0|s_1\rangle,
$$

and the reverse coupling has the same coefficient. All other radial links have coefficients $J_j$, just as in part (c). Thus the [symmetric-arm reduction of an exchange Hamiltonian](../../../../../../symmetric-arm-reduction-of-an-exchange-hamiltonian.md) is again exactly $H_T$. At time $\pi/2$ its evolution is

$$
|s_0\rangle\longmapsto|s_N\rangle=\frac{|1,N\rangle+|2,N\rangle+|3,N\rangle}{\sqrt3}.
$$

Every nontip [qubit](../../../../../../qubit.md) is zero, so tracing them out leaves the three tips in the pure [W state](../../../../../../w-state.md)

$$
\boxed{|W_3\rangle=\frac{|100\rangle+|010\rangle+|001\rangle}{\sqrt3}.}
$$

The essential change is the additional identical arm and the normalization of each hub coupling by $\sqrt3$ instead of $\sqrt2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
