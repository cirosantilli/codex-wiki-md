<h1 id="6g/solution">Solution</h1>

↑ **Parent:** [6G](../6g.md)

For every $u\in U$, write $u=(u-\alpha u)+\alpha u$. The first term lies in $\ker\alpha$, since $\alpha^2=\alpha$, and the second lies in $\operatorname{im}\alpha$. If $v$ belongs to both spaces, write $v=\alpha w$; then $\alpha v=\alpha^2w=\alpha w=v$, whereas membership in the [kernel](../../../../../kernel-of-a-linear-map.md) gives $\alpha v=0$. Thus the intersection is zero and

$$
\boxed{U=\ker\alpha\oplus\operatorname{im}\alpha}.
$$

In a [basis](../../../../../basis.md) assembled from [bases](../../../../../basis.md) of these two spaces, the [idempotent linear map](../../../../../projection-linear-algebra.md) has [matrix](../../../../../matrix.md) $\operatorname{diag}(0_{d-r},I_r)$, where $d=\dim U$ and $r=\operatorname{rank}\alpha$. Therefore

$$
\boxed{\chi_\alpha(t)=t^{d-r}(t-1)^r}.
$$

This [basis](../../../../../basis.md) consists entirely of [eigenvectors](../../../../../eigenvector.md), so **$\alpha$ is diagonalizable over the reals**, including the extreme cases $r=0$ and $r=d$.

## ↑ Ancestors (10)

1. [6G](../6g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
