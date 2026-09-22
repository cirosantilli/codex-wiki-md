<h1 id="17g/solution">Solution</h1>

↑ **Parent:** [17G](../17g.md)

Use the Leibniz definition of the [determinant](../../../../../determinant.md):

$$
\det A=\sum_{\pi\in S_n}\operatorname{sgn}(\pi)\prod_{i=1}^na_{i,\pi(i)}.
$$

For the permuted-column [matrix](../../../../../matrix.md), $a^\sigma_{ij}=a_{i,\sigma(j)}$. Reindex the sum by $\tau=\sigma\circ\pi$. The [sign of a permutation](../../../../../sign-of-a-permutation.md) is multiplicative, so $\operatorname{sgn}(\pi)=\operatorname{sgn}(\sigma)\operatorname{sgn}(\tau)$. It follows directly that

$$
\det(A^\sigma)=\operatorname{sgn}(\sigma)\det A.
$$

For the [matrix transpose](../../../../../transpose.md), the products in its determinant are $\prod_i a_{\pi(i),i}$. Set $j=\pi(i)$ to obtain $\prod_j a_{j,\pi^{-1}(j)}$, and use $\operatorname{sgn}(\pi^{-1})=\operatorname{sgn}(\pi)$. This proves $\det(A^t)=\det A$. These facts also show that equal columns, or equal rows by transposition, force the [determinant](../../../../../determinant.md) to be zero: exchanging the equal pair leaves the matrix unchanged but changes the determinant's sign.

Let $M_{ij}$ be the [matrix](../../../../../matrix.md) obtained by deleting row $i$ and column $j$, with the empty determinant taken as one for $n=1$. Define the cofactor $C_{ij}=(-1)^{i+j}\det M_{ij}$ and the [adjugate matrix](../../../../../adjugate-matrix.md) by $\operatorname{adj}(A)_{ij}=C_{ji}$. Grouping the Leibniz sum according to the column chosen in row $i$ gives the cofactor expansion $\det A=\sum_k a_{ik}C_{ik}$: deleting that row and its chosen column leaves a permutation of $n-1$ entries, with sign factor $(-1)^{i+k}$. Therefore

$$
(A\operatorname{adj}A)_{ij}=\sum_k a_{ik}C_{jk}.
$$

When $i=j$ this is $\det A$. When $i\ne j$ it is the cofactor expansion along row $j$ of the matrix formed by replacing that row with row $i$; its remaining minors are unchanged, and its two equal rows give determinant zero. The column version proves the other product in the same way. Thus the [adjugate identity](../../../../../adjugate-identity.md) is

$$
\boxed{A\operatorname{adj}(A)=\operatorname{adj}(A)A=(\det A)I,\qquad A^{-1}=\frac{\operatorname{adj}(A)}{\det A}\quad(\det A\ne0).}
$$

For the real [matrices](../../../../../matrix.md) $C,D$, let $p(t)=\det(C+tD)$. The determinant definition makes this a real [polynomial](../../../../../polynomial-split.md) of [degree of a polynomial](../../../../../degree-of-a-polynomial.md) at most $n$. Since $C+iD$ is invertible, the allowed converse implies $p(i)\ne0$, so $p$ is not the zero polynomial. It has at most $n$ real [roots of a polynomial](../../../../../root-of-a-polynomial.md). Choose a real $\lambda$ outside those roots; the adjugate argument proves that $C+\lambda D$ is invertible.

Finally write the given complex [similarity transformation](../../../../../similarity-transformation.md) as $P=C+iD$. The relation $AP=PB$, with $A,B$ real, yields $AC=CB$ and $AD=DB$ by comparing real and imaginary parts. Choose the preceding $\lambda$ and put $Q=C+\lambda D$. Then $AQ=QB$, so

$$
\boxed{Q^{-1}AQ=B\quad\text{with }Q\text{ real and invertible}.}
$$

This proves [real similarity from complex similarity](../../../../../real-similarity-from-complex-similarity.md) by constructing a real intertwiner, rather than requiring $C$ or $D$ separately to be invertible.

## ↑ Ancestors (10)

1. [17G](../17g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
