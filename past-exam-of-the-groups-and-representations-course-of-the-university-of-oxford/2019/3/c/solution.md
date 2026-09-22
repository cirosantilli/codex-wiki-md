<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use upper indices for the defining [representation](../../../../group-representation.md) of [SU(6)](../../../../su-6.md) and lower indices for its [dual representation](../../../../dual-representation.md). The [Young tableaux](../../../../young-tableau.md) below display tensor-slot labels; their shapes determine the [Young diagrams](../../../../young-diagram.md). Full columns of height six are [determinant representations](../../../../determinant-representation.md) and can be removed for [SU(6)](../../../../su-6.md).

$$
\begin{array}{c|c|c|c|c}
\text{representation}&\text{Dynkin labels}&\text{tableau}&\text{tensor}&\dim\\\hline
\mathbf6&(1,0,0,0,0)&\boxed{1}&v^a&6\\[3pt]
\overline{\mathbf6}&(0,0,0,0,1)&\begin{array}{l}\boxed{1}\\[-3pt]\boxed{2}\\[-3pt]\boxed{3}\\[-3pt]\boxed{4}\\[-3pt]\boxed{5}\end{array}&w_a&6\\[3pt]
\mathbf{21}&(2,0,0,0,0)&\boxed{1}\boxed{2}&S^{(ab)}&21\\[3pt]
\mathbf{15}&(0,1,0,0,0)&\begin{array}{l}\boxed{1}\\[-3pt]\boxed{2}\end{array}&A^{[ab]}&15\\[3pt]
\mathbf{35}&(1,0,0,0,1)&\begin{array}{l}\boxed{1}\boxed{2}\\[-3pt]\boxed{3}\\[-3pt]\boxed{4}\\[-3pt]\boxed{5}\\[-3pt]\boxed{6}\end{array}&T^a{}_b,\ T^a{}_a=0&35
\end{array}
$$

Here all indices run from one to six. The [highest weight](../../../../highest-weight-of-a-representation.md) [Dynkin labels](../../../../dynkin-label.md) follow from the differences of successive row lengths. In the same order the row lengths are $(1)$, $(1,1,1,1,1)$, $(2)$, $(1,1)$ and $(2,1,1,1,1)$.

The defining [vector](../../../../vector.md) transforms as $v^a\mapsto U^a{}_bv^b$. For a [unitary representation](../../../../unitary-representation.md), the [conjugate representation](../../../../conjugate-representation.md) is equivalent to the [dual representation](../../../../dual-representation.md), so $\overline{\mathbf6}$ can be written as a [covector](../../../../covector.md) with $w_a\mapsto w_b(U^{-1})^b{}_a$. Its five-box column is equivalently a totally [antisymmetric tensor](../../../../antisymmetric-tensor.md) $A^{a_1\cdots a_5}$, related by the invariant alternating [tensor](../../../../tensor.md) $w_a=\epsilon_{aa_1\cdots a_5}A^{a_1\cdots a_5}/5!$.

The [symmetric tensor](../../../../symmetric-tensor.md) transforms as $S^{ab}\mapsto U^a{}_cU^b{}_dS^{cd}$, with $6(6+1)/2=21$ independent components. The [antisymmetric tensor](../../../../antisymmetric-tensor.md) has the same transformation law but obeys $A^{ab}=-A^{ba}$, giving $6(6-1)/2=15$ independent components. For the [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md), $T\mapsto UTU^{-1}$; the [trace](../../../../matrix-trace.md) constraint removes one component from the $36$ entries of a mixed [tensor](../../../../tensor.md), leaving $35$. Its six-box [Young diagram](../../../../young-diagram.md) is obtained by converting the five-index column to a lower index and selecting the traceless mixed [tensor](../../../../tensor.md).

Thus the requested [dimensions](../../../../dimension-vector-space.md), in the order above, are

$$
\boxed{6,\quad6,\quad21,\quad15,\quad35.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
