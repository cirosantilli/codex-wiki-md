<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the [alternating bilinear form](../../../../../../alternating-bilinear-form.md) as $B$. Alternation gives $B(v,w)=-B(w,v)$ by expanding $B(v+w,v+w)=0$. If $V\ne0$, choose $v\ne0$. Nondegeneracy supplies $w$ with $B(v,w)\ne0$; rescale $w$ so that $B(v,w)=1$. The vectors are independent, and the restriction to $E=\operatorname{span}\{v,w\}$ has matrix $\begin{pmatrix}0&1\\-1&0\end{pmatrix}$, whose [determinant](../../../../../../determinant.md) is one.

Every $z\in V$ has a unique decomposition into a vector in $E$ and a vector orthogonal to $E$: subtract $B(z,w)v-B(z,v)w$ to obtain the latter. Thus $V=E\oplus E^\perp$. If a vector in $E^\perp$ annihilates $E^\perp$ under $B$, it also annihilates $E$, and hence all of $V$; nondegeneracy makes it zero. The restricted [alternating bilinear form](../../../../../../alternating-bilinear-form.md) on $E^\perp$ is therefore again nondegenerate. Induction splits off two dimensions at each step and ends at the zero space. Hence

$$
\boxed{\dim V\text{ is even}.}
$$

The proof works in characteristic two as well: alternation, rather than merely skew symmetry, is the needed hypothesis.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
