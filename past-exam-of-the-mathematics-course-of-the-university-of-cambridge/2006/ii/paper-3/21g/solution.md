<h1 id="21g/solution">Solution</h1>

↑ **Parent:** [21G](../21g.md)

If $x_i\rightharpoonup x$ and $\psi\in Y^*$, then $\psi\circ T\in X^*$ because $T$ is bounded and linear. Therefore $\psi(Tx_i)\to\psi(Tx)$, proving weak continuity of $T$.

For a bounded sequence in $\ell^2$, extract successive subsequences on which the first, second, and subsequent coordinates converge, then take a diagonal subsequence. Call the coordinate limits $x_j$. Every finite partial sum satisfies $\sum_{j\le m}|x_j|^2\le1$, so $x\in\ell^2$ and $\|x\|\le1$. For any $h\in\ell^2$, the pairing on its first $m$ coordinates converges, while the pairing on the tail is bounded uniformly by $2\|h_{>m}\|_2$. First choose $m$ large, then take the subsequence limit. The [Riesz representation theorem](../../../../../riesz-representation-theorem.md) identifies these pairings with every [continuous linear functional](../../../../../continuous-linear-functional.md), proving the requested [weak convergence](../../../../../weak-convergence.md).

For $\ell^1$, [norm convergence](../../../../../norm-convergence.md) implies [weak convergence](../../../../../weak-convergence.md) immediately. Conversely, suppose $z_i\rightharpoonup0$ but a subsequence has $\|z_i\|_1\ge\delta>0$. Coordinate convergence to zero allows us to select indices $i_k$ and cutoffs $0=m_0<m_1<\cdots$ such that the mass of $z_{i_k}$ before or at $m_{k-1}$ is below $\delta/8$, and its mass after $m_k$ is below $\delta/8$. Its mass on the intervening block is then at least $3\delta/4$. On that block set $a_j=\overline{z_{i_k,j}}/|z_{i_k,j}|$ when nonzero and zero otherwise. These prescriptions define $a\in\ell^\infty$. The bounded [linear functional](../../../../../linear-functional.md) $z\mapsto\sum_ja_jz_j$ has real part at least $3\delta/4-\delta/4=\delta/2$ on every selected $z_{i_k}$, contradicting [weak convergence](../../../../../weak-convergence.md). Translating by the limit proves **weak and [norm convergence](../../../../../norm-convergence.md) of sequences coincide in $\ell^1$**, the [Schur property](../../../../../schur-property.md).

A [compact operator](../../../../../compact-operator-split.md) sends bounded sets to relatively norm-compact sets. Every bounded sequence in $\ell^2$ has a weakly convergent subsequence by the argument above, after scaling into the unit ball. Its image under $T:\ell^2\to\ell^1$ converges weakly and therefore in norm by the [Schur property](../../../../../schur-property.md). Sequential compactness in a metric space gives relative compactness of the image of the unit ball. **Every [bounded linear operator](../../../../../continuous-linear-operator.md) from $\ell^2$ to $\ell^1$ is compact.**

## ↑ Ancestors (10)

1. [21G](../21g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
