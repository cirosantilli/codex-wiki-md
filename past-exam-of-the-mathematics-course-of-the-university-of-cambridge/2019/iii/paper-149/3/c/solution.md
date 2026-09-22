<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $N=[G,G]$ and identify it with $(\mathbb C,+)$ as in part (a). If every two members of $A$ commuted, then $\langle A\rangle$ would be [Abelian](../../../../../../abelian-group.md), contrary to hypothesis. Thus some commutator of two members of $A$ is a nonidentity translation in $A^4\cap N$. Consequently the translation-coordinate set

$$
T=\{c\in\mathbb C:f_{1,c}\in A^4\cap N\}
$$

contains both zero and a nonzero element.

The identity

$$
f_{a,b}\circ f_{1,c}\circ f_{a,b}^{-1}=f_{1,ac}
$$

shows that $T\pi(A)$ is contained in the translation coordinates of $A^6\cap N$, while $T+T$ is contained in those of $A^8\cap N$. The [intersection of an approximate group power with a subgroup](../../../../../../intersection-of-an-approximate-group-power-with-a-subgroup.md) therefore gives

$$
|T+T|\leq K^{O(1)}|T|,
\qquad
|T\pi(A)|\leq K^{O(1)}|T|.
$$

Apply the [Solymosi sum-product theorem over the complex numbers](../../../../../../solymosi-sum-product-theorem-over-the-complex-numbers.md) with $U=V=T$ and $W=\pi(A)$. Since $1\in\pi(A)$, its hypotheses hold, and

$$
K^{O(1)}|T|^2
\geq |T+T|\,|T\pi(A)|
\geq\frac1{56}|T|^2|\pi(A)|^{1/2}.
$$

Cancelling $|T|^2$ and absorbing the absolute constant proves

$$
\boxed{|\pi(A)|\leq K^{O(1)}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 149](../../../paper-149-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
