<h1 id="20f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the orientations

$$
t=[v_1v_2v_3],
\qquad
e_{ij}=[v_iv_j]\quad(i<j).
$$

The [simplicial chain complex](../../../../../../simplicial-chain-complex.md) has

$$
C_2\cong\mathbb Z,
\qquad C_1\cong\mathbb Z^5,
\qquad C_0\cong\mathbb Z^4,
$$

with

$$
\partial_2t=e_{23}-e_{13}+e_{12},
\qquad
\partial_1e_{ij}=v_j-v_i.
$$

The map $\partial_2$ is injective, so $H_2(K)=0$. The complex is connected, so $H_0(K)\cong\mathbb Z$ and $\operatorname{rank}\partial_1=3$. Hence $\ker\partial_1$ has rank $5-3=2$; quotienting by the rank-one primitive subgroup $\operatorname{im}\partial_2$ gives

$$
H_1(K)\cong\mathbb Z.
$$

There are no higher simplices. Therefore

$$
H_n(K)\cong
\begin{cases}
\mathbb Z,&n=0,1,\\
0,&n\geq2.
\end{cases}
$$

The result agrees with the [Euler characteristic](../../../../../../euler-characteristic.md) $4-5+1=0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20F](../../20f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
