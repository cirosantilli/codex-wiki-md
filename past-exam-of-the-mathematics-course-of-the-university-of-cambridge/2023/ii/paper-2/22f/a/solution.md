<h1 id="22f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
m=\frac{v+w}{2},
\qquad
R(z)=v+w-z=2m-z.
$$

The map $R$ is reflection about $m$ and is an isometry. It interchanges $v,w$, so it preserves $S_1^{vw}$. Inductively, if it preserves $S_{n-1}^{vw}$, then it preserves its [diameter](../../../../../../diameter.md) and all distances in the defining condition for $S_n^{vw}$; hence it preserves every $S_n^{vw}$.

The midpoint belongs to $S_1^{vw}$ because

$$
\|m-v\|=\|m-w\|=\frac12\|v-w\|.
$$

Suppose $m\in S_{n-1}^{vw}$. For every $z\in S_{n-1}^{vw}$, reflection invariance gives $R(z)\in S_{n-1}^{vw}$ and

$$
\|m-z\|
=\frac12\|R(z)-z\|
\leq\frac12\operatorname{diam}(S_{n-1}^{vw}).
$$

Thus $m\in S_n^{vw}$, so all the sets are nonempty and contain $m$.

Put $D_n=\operatorname{diam}(S_n^{vw})$. If $x,y\in S_n^{vw}$ with $n\geq2$, then $y\in S_{n-1}^{vw}$ and the defining property of $x$ gives

$$
\|x-y\|\leq\frac12D_{n-1}.
$$

Therefore

$$
D_n\leq\frac12D_{n-1},
\qquad
D_n\leq2^{1-n}D_1\longrightarrow0.
$$

If $z$ lies in every $S_n^{vw}$, then both $z$ and $m$ lie in $S_n^{vw}$, so

$$
\|z-m\|\leq D_n\longrightarrow0.
$$

Hence $z=m$. We have proved the [metric extraction of a midpoint by shrinking diameters](../../../../../../metric-extraction-of-a-midpoint-by-shrinking-diameters.md):

$$
\boxed{\bigcap_{n\geq1}S_n^{vw}
=\left\{\frac{v+w}{2}\right\}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22F](../../22f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
