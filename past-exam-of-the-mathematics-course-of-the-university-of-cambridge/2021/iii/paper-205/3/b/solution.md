<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply part a to each of the at most $n(n-1)/2$ nonzero differences $u_i-u_j$. For $w_i=Au_i/\sqrt d$, the [union bound](../../../../../../boole-s-inequality.md) makes the probability of any failure at most

$$
\frac{n(n-1)}2\,2e^{-dt^2/136}
<n^2e^{-dt^2/136}.
$$

The assumed inequality $d>272\log(n/\sqrt\varepsilon)/t^2$ makes this smaller than $\varepsilon$. Hence, simultaneously for every distinct pair,

$$
1-t\leq\frac{\lVert w_i-w_j\rVert_2^2}{\lVert u_i-u_j\rVert_2^2}\leq1+t
$$

with probability at least $1-\varepsilon$, which is the finite-set [Johnson–Lindenstrauss lemma](../../../../../../johnson-lindenstrauss-lemma.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
