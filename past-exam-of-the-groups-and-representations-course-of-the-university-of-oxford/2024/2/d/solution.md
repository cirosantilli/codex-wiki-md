<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The embedded $SU(3)$ acts on the first three coordinates and fixes the fourth. This immediately gives the [branching rules](../../../../branching-rule.md)

$$
\boxed{\mathbf4\downarrow SU(3)=\mathbf3\oplus\mathbf1,\qquad
\bar{\mathbf4}\downarrow SU(3)=\bar{\mathbf3}\oplus\mathbf1.}
$$

Distribute the [tensor product of group representations](../../../../tensor-product-of-group-representations.md) over these [direct sums](../../../../direct-sum.md) and split $\mathbf3\otimes\bar{\mathbf3}=\mathbf8\oplus\mathbf1$ by taking the [trace](../../../../matrix-trace.md):

$$
\boxed{(\mathbf4\otimes\bar{\mathbf4})\downarrow SU(3)
=\mathbf8\oplus\mathbf3\oplus\bar{\mathbf3}\oplus\mathbf1\oplus\mathbf1.}
$$

One can locate every summand using the block [matrix](../../../../matrix.md)

$$
M=\begin{pmatrix}A&b\\c&d\end{pmatrix}
\longmapsto
\begin{pmatrix}U_3AU_3^\dagger&U_3b\\cU_3^\dagger&d\end{pmatrix}.
$$

The traceless part of $A$ is $\mathbf8$, $b$ is $\mathbf3$, $c$ is $\bar{\mathbf3}$, and $\operatorname{tr}A,d$ are independent [trivial representations](../../../../trivial-representation.md). Removing the overall [trace](../../../../matrix-trace.md) instead gives $\mathbf{15}\downarrow SU(3)=\mathbf8\oplus\mathbf3\oplus\bar{\mathbf3}\oplus\mathbf1$. The dimension check is $16=8+3+3+1+1$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
