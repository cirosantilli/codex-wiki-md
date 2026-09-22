<h1 id="8g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $I\subseteq[m]$, the independent [vectors](../../../../../../vector.md) $\{v_i:i\in I\}$ lie in the coordinate subspace supported on

$$
S_I=\bigcup_{i\in I}\operatorname{supp}(v_i),
$$

which has dimension $|S_I|$. Hence $|I|\leq|S_I|$, and the stated form of [Hall marriage theorem](../../../../../../hall-s-marriage-theorem.md) gives an injection $f$ with $f(i)\in\operatorname{supp}(v_i)$.

Let $V$ be the $n\times m$ [matrix](../../../../../../matrix.md) whose $i$th column is $v_i$. Its column rank is $m$. By equality of row and column rank, it has $m$ linearly independent rows. Let $B$ be their indices. The $m\times m$ submatrix $V_B$ is invertible, so its columns are independent. Those columns are exactly the nonzero coordinates of $Bv_1,\ldots,Bv_m$, and therefore these truncated [vectors](../../../../../../vector.md) are linearly independent.

Expanding $\det V_B$ gives a permutation $f:[m]\to B$ for which

$$
\prod_{i=1}^m (v_i)_{f(i)}\ne0.
$$

Thus $f(i)\in\operatorname{supp}(v_i)$. Finally, order the coordinates with $B$ first. The [matrix](../../../../../../matrix.md) whose columns are the $v_i$ together with the $e_j$ for $j\notin B$ is block triangular, with diagonal blocks $V_B$ and an identity [matrix](../../../../../../matrix.md). Its [determinant](../../../../../../determinant.md) is nonzero. Consequently

$$
\boxed{
\bigl(\{e_j:j\in[n]\}\setminus\{e_{f(i)}:i\in[m]\}\bigr)
\cup\{v_i:i\in[m]\}
}
$$

is a [basis](../../../../../../basis.md) of $\mathbb C^n$. This is the [simultaneous basis exchange from a nonzero minor](../../../../../../simultaneous-basis-exchange-from-a-nonzero-minor.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8G](../../8g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
