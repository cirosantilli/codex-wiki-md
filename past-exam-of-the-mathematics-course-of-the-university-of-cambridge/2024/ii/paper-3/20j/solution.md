<h1 id="20j/solution">Solution</h1>

↑ **Parent:** [20J](../20j.md)

Because $K$ is a subcomplex, $\partial C_k(K)\subseteq C_{k-1}(K)$, so

$$
\partial(c+C_k(K))=\partial c+C_{k-1}(K)
$$

is well defined and squares to zero. The short exact [sequence](../../../../../sequence.md) of chain complexes

$$
0\to C_\bullet(K)\to C_\bullet(L)\to C_\bullet(L,K)\to0
$$

gives the long exact [sequence](../../../../../sequence.md)

$$
\cdots\to H_k(K)\to H_k(L)\to H_k(L,K)
\to H_{k-1}(K)\to\cdots.
$$

Taking $L=\partial\Delta^{n+1}$ and using the contractibility of $\Delta^{n+1}$ gives

$$
H_k(\partial\Delta^{n+1})\cong
\begin{cases}\mathbb Z,&k=0,n,\\0,&\text{otherwise}.
\end{cases}
$$

For $0<k<n$, exactness makes $H_k(K)$ a quotient of a [subgroup](../../../../../subgroup.md) of $H_{k+1}(L,K)$, whose rank is at most

$$
\operatorname{rank}C_{k+1}(L,K)
=\binom{n+2}{k+2}-\#\{(k+1)\text{-simplices of }K\}.
$$

The same stated inequality for $k=n$ follows from $H_n(K)\hookrightarrow H_n(L)\cong\mathbb Z$. Finally, an $n$-cycle in the boundary sphere has equal signed coefficients on all $n$-faces. A proper subcomplex omits an $n$-face, so that coefficient and hence every coefficient is zero. Therefore $H_n(K)=0$.

## ↑ Ancestors (10)

1. [20J](../20j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
