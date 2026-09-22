<h1 id="28j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $d_G(x)$ for the degree of $x$ in $G$ and $d_A(x)$ for the number of its neighbours lying in $A$. Each trial succeeds with probability  
$d_A(x)/d_G(x)$. The stated geometric-sum fact shows that the total holding time at $x$ is exponential with rate $d_A(x)/d_G(x)$. Conditional on success, each neighbour in $A$ is chosen uniformly. Hence

$$
\boxed{q_{xy}=
\begin{cases}
1/d_G(x),&xy\in E(A),\\
0,&x\ne y,\ xy\notin E(A),
\end{cases}
\qquad
q_{xx}=-d_A(x)/d_G(x)}.
$$

Let

$$
\pi(x)=\frac{d_G(x)}{\sum_{z\in A}d_G(z)}.
$$

For every edge $xy$ of $A$,

$$
\pi(x)q_{xy}
=\frac1{\sum_{z\in A}d_G(z)}
=\pi(y)q_{yx}.
$$

**Thus [detailed balance](../../../../../../detailed-balance.md) holds, so $\pi$ is invariant. Connectedness of $A$ makes the chain irreducible and this invariant distribution unique.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28J](../../28j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
