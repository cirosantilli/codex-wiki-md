<h1 id="s03/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Expand a normalized [product state](../../../../../product-state.md) as

$$
(a|0\rangle+b|1\rangle)\otimes(c|0\rangle+d|1\rangle)
=ac|00\rangle+ad|01\rangle+bc|10\rangle+bd|11\rangle.
$$

Thus $\alpha=ac$, $\beta=ad$, $\gamma=bc$, $\delta=bd$, giving

$$
\boxed{\alpha\delta=abcd=\beta\gamma.}
$$

Conversely the nonzero coefficient matrix $C=\begin{pmatrix}\alpha&\beta\\\gamma&\delta\end{pmatrix}$ has determinant zero precisely when it has rank one, so the condition also suffices for a pure [two-qubit state](../../../../../two-qubit-state.md) to factor.

For any fixed pair of local measurement settings with operators $E_i,F_j$, the [Born rule](../../../../../born-rule.md) factorizes:

$$
\boxed{p(i,j)=\langle a|E_i|a\rangle\langle b|F_j|b\rangle=p_A(i)p_B(j).}
$$

Hence a [product state](../../../../../product-state.md) has independent local results in every pair of local bases. This assumes independent settings and local measurements; shared classical randomization of preparations or a subsequent joint interaction can generate correlations. A separable mixture is not necessarily a single [product state](../../../../../product-state.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [S03](../../../s03.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
