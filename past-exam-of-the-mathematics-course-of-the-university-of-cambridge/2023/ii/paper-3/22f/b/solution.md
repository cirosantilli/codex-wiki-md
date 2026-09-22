<h1 id="22f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Extend $u_k$ and $u$ by zero outside the bounded set $U$. Weak convergence makes $(u_k)$ bounded in $L^2(U)$. For each fixed $p$,

$$
\widehat u_k(p)=\int_Uu_k(x)e^{-ip\cdot x}\,dx
\longrightarrow
\int_Uu(x)e^{-ip\cdot x}\,dx
=\widehat u(p),
$$

because $e^{-ip\cdot x}\in L^2(U)$.

Fix $t>0$. On the finite-measure ball $|p|\leq t$, the Fourier transforms are uniformly bounded by

$$
|\widehat u_k(p)-\widehat u(p)|
\leq |U|^{1/2}\|u_k-u\|_2.
$$

Dominated convergence therefore gives

$$
\int_{|p|\leq t}|\widehat u_k-\widehat u|^2\,dp\to0.
$$

On the complementary region,

$$
|\widehat u_k-\widehat u|^2
\leq2(|\widehat u_k|^2+|\widehat u|^2),
$$

whose integral tends to zero uniformly in $k$ as $t\to\infty$ by hypothesis. Splitting first at large $t$ and then taking $k\to\infty$, the [Plancherel theorem](../../../../../../plancherel-theorem.md) yields

$$
\boxed{\|u_k-u\|_{L^2(U)}\to0.}
$$

This is the same low-frequency compactness mechanism used in the [Fourier proof of Rellich compactness](../../../../../../fourier-proof-of-rellich-compactness.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22F](../../22f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
