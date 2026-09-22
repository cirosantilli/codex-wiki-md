<h1 id="20f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [covering space](../../../../../../covering-space.md) is a map $p:\widetilde X\to X$ such that every $x\in X$ has an open neighbourhood $U$ for which

$$
p^{-1}(U)=\bigsqcup_{\lambda}U_\lambda,
$$

with every restriction $p:U_\lambda\to U$ a homeomorphism.

Let $N=\langle\!\langle a\rangle\!\rangle$ in  
$\pi_1(Y)=\langle a,b\mid a^2b^{-3}\rangle$. Then

$$
\pi_1(Y)/N\cong\langle b\mid b^3=1\rangle\cong C_3.
$$

The subgroup is normal of index three, so the [degree of a connected covering](../../../../../../degree-of-a-connected-covering.md) shows that every fibre $p^{-1}(y)$ has exactly three points.

The [cell complex of a covering from a coset graph](../../../../../../cell-complex-of-a-covering-from-a-coset-graph.md) gives an explicit model. Take vertices $v_0,v_1,v_2$ with indices modulo three; put an $a$-loop $A_i$ at every $v_i$, and a directed $b$-edge $B_i:v_i\to v_{i+1}$. Attach a 2-cell at each $v_i$ along

$$
A_i^2B_{i-1}^{-1}B_{i-2}^{-1}B_i^{-1}.
$$

Map every $v_i$ to $y_0$, every $A_i$ to the $a$-cell, every $B_i$ to the $b$-cell, and each 2-cell homeomorphically to the unique 2-cell of $Y$. Its attaching word is the lift of $a^2b^{-3}$ beginning at $v_i$. This defines the required connected three-sheeted covering.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20F](../../20f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
