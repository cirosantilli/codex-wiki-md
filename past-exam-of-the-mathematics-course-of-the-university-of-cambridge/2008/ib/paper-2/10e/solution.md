<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

The [determinant](../../../../../determinant.md) is

$$
\det A=\sum_{\sigma\in S_n}\operatorname{sgn}(\sigma)\prod_{i=1}^n a_{i,\sigma(i)}.
$$

Equivalently it is the alternating multilinear function of the columns with value one on the identity matrix. To prove multiplicativity, write column $j$ of $AB$ as $\sum_k b_{kj}A_k$, where $A_k$ is column $k$ of $A$. Multilinear expansion gives a sum over choices $k_1,\ldots,k_n$; terms with repeated choices vanish by alternation. The remaining permutations contribute

$$
\det(AB)=\det A\sum_{\sigma\in S_n}\operatorname{sgn}(\sigma)\prod_jb_{\sigma(j),j}
=\boxed{\det A\det B}.
$$

If $C$ is invertible, $CB=C(BC)C^{-1}$, so multiplicativity makes $\det(CBC^{-1}-\lambda I)=\det(BC-\lambda I)$ and $p_{CB}=p_{BC}$. For arbitrary $A$, put $C=A+tI$. Its [determinant](../../../../../determinant.md) is a nonzero polynomial in $t$, so it is invertible except for finitely many values. Thus for all other $t$,

$$
p_{B(A+tI)}(\lambda)=p_{(A+tI)B}(\lambda).
$$

For each fixed $\lambda$ both sides are polynomials in $t$, and equality at infinitely many $t$ makes them identical. Setting $t=0$ proves the [Characteristic polynomials of AB and BA](../../../../../characteristic-polynomials-of-ab-and-ba.md) identity $\boxed{p_{BA}=p_{AB}}$ without an invertibility assumption on $A$.

In the convention $p_A(\lambda)=\det(A-\lambda I)$, the coefficient of $\lambda^{n-1}$ is $(-1)^{n-1}\operatorname{tr}A$: in the [determinant](../../../../../determinant.md) expansion such a term chooses one diagonal entry of $A$ and $n-1$ factors $-\lambda$; nonidentity permutations have at least two nonfixed positions and contribute lower degree. Therefore $\boxed{p_A=p_B\implies\operatorname{tr}A=\operatorname{tr}B}$.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
