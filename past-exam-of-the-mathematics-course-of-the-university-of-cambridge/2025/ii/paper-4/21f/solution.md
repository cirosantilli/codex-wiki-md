<h1 id="21f/solution">Solution</h1>

↑ **Parent:** [21F](../21f.md)

The [universal coefficient theorem for homology](../../../../../universal-coefficient-theorem-for-homology.md) and flatness of $\mathbb Q$ give

$$
H_i(X;\mathbb Q)
\cong H_i(X;\mathbb Z)\otimes_\mathbb Z\mathbb Q.
$$

Thus, if

$$
H_i(X;\mathbb Z)\cong\mathbb Z^{b_i}\oplus T_i
$$

with $T_i$ torsion, then $H_i(X;\mathbb Q)\cong\mathbb Q^{b_i}$.

For a finite triangulable space, its [Euler characteristic](../../../../../euler-characteristic.md) is

$$
\chi(X)=\sum_i(-1)^i\dim_\mathbb QH_i(X;\mathbb Q).
$$

If $K$ is a finite triangulation and $f_i$ is its number of $i$-simplices, then the [Euler-Poincare formula](../../../../../euler-poincare-formula.md) is

$$
\chi(X)=\sum_i(-1)^if_i.
$$

To prove it over $\mathbb Q$, write $Z_i=\ker\partial_i$ and $B_i=\operatorname{im}\partial_{i+1}$. Rank-nullity and $H_i=Z_i/B_i$ give

$$
\dim C_i
=\dim Z_i+\dim B_{i-1}
=\dim H_i+\dim B_i+\dim B_{i-1}.
$$

After multiplying by $(-1)^i$ and summing, the two boundary sums cancel, leaving the claimed equality.

The standard simplex $\Delta^3$ is contractible, so

$$
H_i(\Delta^3)\cong
\begin{cases}
\mathbb Z,&i=0,\\
0,&i>0.
\end{cases}
$$

## ↑ Ancestors (10)

1. [21F](../21f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
