<h1 id="22i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $C(K)=\bigcup_{n\geq1}\mathcal S_n$ with every $\mathcal S_n$ equicontinuous. Its closure $E_n=\overline{\mathcal S_n}$ is still equicontinuous, because [uniform limits](../../../../../../uniform-limit.md) preserve the same oscillation inequalities. The [Baire category theorem](../../../../../../baire-category-theorem.md) applied to the [Banach space](../../../../../../banach-space-split.md) $C(K)$ shows that some $E_n$ has nonempty interior. Hence there are $f_0\in C(K)$ and $r>0$ such that the open ball $B(f_0,r)$ lies in $E_n$.

Fix $x\in K$. Equicontinuity of $E_n$ gives a neighborhood $U$ of $x$ on which every member of $E_n$ changes by less than $r/4$. If $y\in U$ were distinct from $x$, the [normality of a compact Hausdorff space](../../../../../../normality-of-a-compact-hausdorff-space.md) and the [Urysohn lemma](../../../../../../urysohn-s-lemma.md) would give $h\in C(K)$ with $h(x)=0$, $h(y)=r/2$, and $\lVert h\rVert_\infty=r/2$. Both $f_0$ and $f_0+h$ belong to $E_n$, yet

$$
|h(y)-h(x)|\leq |(f_0+h)(y)-(f_0+h)(x)|+|f_0(y)-f_0(x)|<r/2,
$$

a contradiction. Thus $U=\{x\}$, so every point is [isolated](../../../../../../isolated-point.md) and $K$ is a [discrete space](../../../../../../discrete-space.md). A compact discrete space is finite, since its cover by singleton open sets has a finite subcover.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22I](../../22i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
