<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Again let $v_i\in\mathbb F_2^n$ be the characteristic vectors. They all lie in the even-weight subspace

$$
E=\{v\in\mathbb F_2^n:v\mathbin\cdot\mathbf1=0\},
$$

which has [dimension](../../../../../../dimension-vector-space.md) $n-1$. Their [Gram matrix](../../../../../../gram-matrix.md) is

$$
G=(v_i\mathbin\cdot v_j)_{i,j}=J_m+I_m,
$$

because its diagonal entries are zero and its off-diagonal entries are one. If $Gx=0$ and $s=\sum_i x_i$, then $x=s\mathbf1$. Consequently

$$
\operatorname{rank}G=
\begin{cases}
m,&m\text{ even},\\
m-1,&m\text{ odd}.
\end{cases}
$$

Since $G=VV^T$ for a matrix whose rows lie in $E$, its rank is at most $n-1$. If $n$ is even, an even $m$ cannot reach $n$, while an odd $m$ is at most $n-1$; hence $m\leq n-1$. If $n$ is odd, the same calculation gives $m\leq n$.

Both bounds are sharp. For odd $n$, take $A_i=[n]\setminus\{i\}$ for $1\leq i\leq n$: each set has even size and two distinct sets meet in the odd number $n-2$. For even $n$, apply the same construction to $[n-1]$ and regard the resulting $n-1$ sets as subsets of $[n]$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
