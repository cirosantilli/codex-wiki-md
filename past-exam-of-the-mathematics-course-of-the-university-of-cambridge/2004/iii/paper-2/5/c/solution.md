<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Translation $X\mapsto I+X$ is a [bijection](../../../../../../bijection.md) from [nilpotent matrices](../../../../../../nilpotent-matrix.md) to [unipotent matrices](../../../../../../unipotent-matrix.md). We can count the former without requiring a further partition identity. Let $a_n$ be their number, with $a_0=1$.

Every [linear operator](../../../../../../linear-operator.md) $T$ has a unique decomposition from the [Fitting lemma](../../../../../../fitting-lemma.md)

$$
V=\ker T^n\oplus\operatorname{im}T^n,
$$

on which it is respectively nilpotent and invertible. To justify the decomposition, kernels and images stabilize by step $n$; if $T^nv\in\ker T^n$, then $v\in\ker T^{2n}=\ker T^n$, so $T^nv=0$. The dimensions then show the sum is all of $V$, and stabilization makes $T$ invertible on the [image](../../../../../../image-of-a-function.md). These two summands are determined by $T$, so there is no overcounting.

For a nilpotent summand of dimension $k$, the number of ordered complementary subspaces is $|GL_n(q)|/(|GL_k(q)||GL_{n-k}(q)|)$, by transporting two fixed bases. The restrictions of $T$ have $a_k$ and $|GL_{n-k}(q)|$ choices. Summing all $q^{n^2}$ [matrices](../../../../../../matrix.md) gives

$$
\frac{q^{n^2}}{|GL_n(q)|}=\sum_{k=0}^n\frac{a_k}{|GL_k(q)|}.
$$

Write $\phi_n(q^{-1})=\prod_{i=1}^n(1-q^{-i})$, so $|GL_n(q)|=q^{n^2}\phi_n(q^{-1})$. Subtract the same equation for $n-1$:

$$
\frac{a_n}{|GL_n(q)|}=\frac1{\phi_n(q^{-1})}-\frac1{\phi_{n-1}(q^{-1})}
=\frac{q^{-n}}{\phi_n(q^{-1})}.
$$

Thus [counting nilpotent matrices by the Fitting decomposition](../../../../../../counting-nilpotent-matrices-by-the-fitting-decomposition.md) proves

$$
\boxed{\#\{\text{unipotent elements of }GL_n(q)\}=a_n=q^{n^2-n}.}
$$

The supplied product identity is consistent with the resulting mass series: taking its variables to be $s=u$, $t=q^{-1}$ gives $\sum_na_nu^n/|GL_n(q)|=\prod_{i\ge1}(1-uq^{-i})^{-1}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
