<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Von Neumann double commutant theorem](../../../../../../von-neumann-double-commutant-theorem.md) states that for a unital star-subalgebra $A\subseteq B(H)$,

$$
\boxed{\overline A^{\mathrm{SOT}}=\overline A^{\mathrm{WOT}}=A''.}
$$

The [commutant of an operator algebra](../../../../../../commutant-of-an-operator-algebra.md) consists of operators commuting with every element. Each commutation equation is closed in the [weak operator topology](../../../../../../weak-operator-topology.md), so $A''$ is weakly closed and contains both indicated closures.

Let $T\in A''$ and fix $\xi_1,\ldots,\xi_m\in H$. On $H^m$ let $A$ act diagonally and put $\xi=(\xi_1,\ldots,\xi_m)$. The subspace $K=\overline{\{(a\xi_1,\ldots,a\xi_m):a\in A\}}$ reduces the diagonal star-algebra. Its [orthogonal projection](../../../../../../orthogonal-projection.md) $P$ therefore commutes with every diagonal $a$. Writing $P$ as an $m\times m$ operator matrix shows that each entry belongs to $A'$. Since $T\in A''$, the diagonal $T$ commutes with $P$. Unitality gives $\xi\in K$, so $P\xi=\xi$ and $P(T\xi)=T\xi$. Thus $T\xi\in K$. By definition of $K$, for any $\varepsilon>0$ a single $a\in A$ satisfies $\sum_j\|(T-a)\xi_j\|^2<\varepsilon^2$. These are precisely the finite-vector neighbourhoods of the [strong operator topology](../../../../../../strong-operator-topology.md). Hence $T$ belongs to the strong closure, completing the proof. Unitality, or the corresponding nondegeneracy hypothesis, is essential to the theorem's stated form.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
