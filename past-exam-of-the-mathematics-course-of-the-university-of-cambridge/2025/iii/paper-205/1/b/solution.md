<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Only the $k$th block can have nonzero subgradient coordinates. If $\beta^{(k)}\ne0$, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) shows that the unique supporting vector is $\beta^{(k)}/\lVert\beta^{(k)}\rVert_2$. At zero, the defining inequality is $\lVert h\rVert_2\geq u^Th$ for every block vector $h$, which is equivalent to $\lVert u\rVert_2\leq1$. Thus

$$
\partial f_k(\beta)=
\begin{cases}
\{u:u^{(j)}=0\ (j\ne k),\ u^{(k)}=\beta^{(k)}/\lVert\beta^{(k)}\rVert_2\},&\beta^{(k)}\ne0,\\
\{u:u^{(j)}=0\ (j\ne k),\ \lVert u^{(k)}\rVert_2\leq1\},&\beta^{(k)}=0.
\end{cases}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
