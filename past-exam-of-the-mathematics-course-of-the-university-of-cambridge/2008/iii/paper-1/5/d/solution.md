<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $F=\ker(I-U)$. For a [unitary operator](../../../../../../unitary-operator.md), $\ker(I-U^*)=F$, so

$$
H=F\oplus\overline{\operatorname{Ran}(I-U)}.
$$

This follows from the general identity $\operatorname{Ran}(A)^\perp=\ker A^*$. The averaging operators have $\|T_n\|\leq1$ and equal the identity on $F$. On a [vector](../../../../../../vector.md) $(I-U)\eta$, telescoping gives

$$
T_n(I-U)\eta=\frac{I-U^n}{n}\eta,\qquad
\|T_n(I-U)\eta\|\leq\frac{2\|\eta\|}{n}\longrightarrow0.
$$

The uniform [norm](../../../../../../norm.md) bound extends this convergence to the [closure](../../../../../../closure-topology.md) of the range. Thus $T_n$ tends to identity on $F$ and to zero on its [orthogonal complement](../../../../../../orthogonal-complement.md). Consequently

$$
\boxed{T_n\xi\longrightarrow P\xi\quad\text{for every }\xi\in H,}
$$

which is exactly convergence in the [strong operator topology](../../../../../../strong-operator-topology.md). This proves the [Von Neumann mean ergodic theorem](../../../../../../von-neumann-mean-ergodic-theorem.md) in the requested unitary case.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
