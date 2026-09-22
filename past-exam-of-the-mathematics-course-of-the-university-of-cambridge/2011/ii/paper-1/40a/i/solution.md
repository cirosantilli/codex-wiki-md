<h1 id="40a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $b$ to be the vector of $f_{ij}$ and absorb $h^{-2}$ into $A$. Its diagonal entry is $-10/(3h^2)$, each axial-neighbour entry is $2/(3h^2)$ and each diagonal-neighbour entry is $1/(6h^2)$. Since these weights agree in both directions, $A$ is a [symmetric matrix](../../../../../../symmetric-matrix.md).

Extend a grid vector $u$ by zero to the whole integer lattice. Let $\mathcal E_a$ contain unordered axial-neighbour pairs and $\mathcal E_d$ unordered diagonal-neighbour pairs. Only finitely many differences involving nonzero values contribute. Each lattice vertex has total neighbour weight $4(2/3)+4(1/6)=10/3$, so expanding the squared differences gives

$$
\boxed{u^TAu=-\frac1{h^2}\left[\frac23\sum_{\{v,w\}\in\mathcal E_a}(u_v-u_w)^2+\frac16\sum_{\{v,w\}\in\mathcal E_d}(u_v-u_w)^2\right].}
$$

It is nonpositive. If it vanishes, every axial difference vanishes. The axial lattice is connected and $u$ is zero outside the finite interior square, forcing $u=0$. Thus $u^TAu<0$ for every nonzero $u$: $\boxed{A\text{ is negative definite}}$.

Reordering the grid replaces $A$ by $P^TAP$ for a [permutation matrix](../../../../../../permutation-matrix.md) $P$. This preserves symmetry and the sign of the quadratic form, proving the assertion for any ordering. Multiplying the whole system by $h^2$ merely rescales $A$ by a positive number and has the same conclusions.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [40A](../../40a.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
