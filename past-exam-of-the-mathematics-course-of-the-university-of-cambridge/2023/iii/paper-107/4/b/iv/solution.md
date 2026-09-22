<h1 id="4/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Fix $B\Subset\Omega$ and $x_0\in B$. Choose $u_j$ in the Perron family with $u_j(x_0)\uparrow\overline u(x_0)$, replace successive terms by finite maxima using part (i), and take their harmonic lifts on $B$. The lifts remain in the family, are increasing, and are uniformly bounded. Interior estimates and the [Arzelà-Ascoli theorem](../../../../../../../arzela-ascoli-theorem.md) give a harmonic limit $h$ on $B$ with $h\leq\overline u$ and $h(x_0)=\overline u(x_0)$.

If $h(y)<\overline u(y)$ somewhere in $B$, take another family member larger than $h(y)$ and repeat the maximum-and-lift construction. Its harmonic limit $H$ satisfies $H\geq h$ and $H(x_0)=h(x_0)$. The [strong minimum principle for elliptic operators](../../../../../../../strong-minimum-principle-for-elliptic-operators.md) forces $H=h$, contradicting the strict inequality at $y$. Thus $h=\overline u$ on $B$. Since $B$ was arbitrary, $\overline u$ is smooth and harmonic in $\Omega$. This is the [Perron method for the Dirichlet problem](../../../../../../../perron-method.md).

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
