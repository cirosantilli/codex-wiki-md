<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the four cyclic factors as $A=M_{ij}$, $B=M_{jk}$, $C=M_{kl}$ and $D=M_{li}$. The [Gaussian moment pairing theorem](../../../../../isserlis-s-theorem.md) gives three terms, corresponding to $(AB)(CD)$, $(AC)(BD)$ and $(AD)(BC)$. We sum each term over $i,j,k,l$.

For $(AB)(CD)$, the entry [covariance](../../../../../covariance.md) gives

$$
\begin{aligned}
\sum_{i,j,k,l}\mathbb E[AB]\mathbb E[CD]
&=\sum_{i,j,k,l}(\delta_{ik}+\delta_{ij}\delta_{jk})
(\delta_{ik}+\delta_{kl}\delta_{li})\\
&=n^3+2n^2+n.
\end{aligned}
$$

Indeed the four products leave respectively three, two, two and one free indices. A cyclic relabelling gives exactly the same sum for $(AD)(BC)$.

For the crossing pairing $(AC)(BD)$,

$$
\begin{aligned}
\sum_{i,j,k,l}\mathbb E[AC]\mathbb E[BD]
&=\sum_{i,j,k,l}(\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk})
(\delta_{jl}\delta_{ki}+\delta_{ji}\delta_{kl})\\
&=n^2+3n.
\end{aligned}
$$

The first product allows $i=k$ and $j=l$ freely, whereas each other product forces all four indices to coincide. Combining the three pairings and the [trace](../../../../../matrix-trace.md) normalization,

$$
\boxed{\mathbb E[m_4(n)]
=\frac{2(n^3+2n^2+n)+(n^2+3n)}{n^3}
=2+\frac5n+\frac5{n^2}\ \longrightarrow\ 2.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
