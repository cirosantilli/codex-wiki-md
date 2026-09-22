<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Consider a depth-$D$ circuit whose gates have range at most $r$. Under backward Heisenberg evolution, a one-site observable has a [backward light cone of a local quantum circuit](../../../../../../backward-light-cone-of-a-local-quantum-circuit.md) of radius at most $rD$. Choose sites $i,j$ separated by $L>2rD$. Their two backward light cones are disjoint. Since the input is a [product state](../../../../../../product-state.md), expectations factorize, and hence every [connected correlation function](../../../../../../connected-correlation-function.md) between the two output observables vanishes.

For the [GHZ state](../../../../../../greenberger-horne-zeilinger-state.md)

$$
|\operatorname{GHZ}_N\rangle
=\frac{|0\rangle^{\otimes N}+|1\rangle^{\otimes N}}{\sqrt2},
$$

however,

$$
\langle Z_i\rangle=\langle Z_j\rangle=0,
\qquad
\langle Z_iZ_j\rangle=1,
\qquad
\langle Z_iZ_j\rangle_c=1
$$

at every separation. The light cones must therefore overlap, which forces

$$
D\geq\frac{L}{2r}.
$$

For opposite ends of a one-dimensional chain, $L=\Theta(N)$, so $D=\Omega(N)$ and no constant-depth local circuit can prepare the GHZ state. The continuous-time version follows directly from the [Lieb-Robinson bound](../../../../../../lieb-robinson-bound.md), with preparation time at least $L/(2v_{\rm LR})$ up to exponentially small tails.

This is the [GHZ-state circuit-depth lower bound](../../../../../../ghz-state-circuit-depth-lower-bound.md). [Finite-depth local circuits](../../../../../../finite-depth-local-quantum-circuit.md) define equivalence within a gapped phase, so a state with this [long-range order](../../../../../../long-range-order.md) cannot lie in the same circuit phase as a product state. The GHZ state is the finite-size cat state associated with spontaneous symmetry breaking; it is not a unique short-range-entangled ground state. The persistent distant correlation is precisely the obstruction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
