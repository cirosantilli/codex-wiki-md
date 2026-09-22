<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $r=g_1=\operatorname{diag}(\alpha,\alpha^2)$ and $s=g_2$, using $\alpha^*=\alpha^{-1}=\alpha^2$. Then

$$
r^3=s^2=I_2,\qquad srs=r^{-1}.
$$

Every word can therefore be put in the form $r^k$ or $r^ks$, with $k=0,1,2$. These give six distinct [matrices](../../../../matrix.md):

$$
\boxed{\begin{aligned}
G=\bigg\{&\begin{pmatrix}1&0\\0&1\end{pmatrix},
\begin{pmatrix}\alpha&0\\0&\alpha^2\end{pmatrix},
\begin{pmatrix}\alpha^2&0\\0&\alpha\end{pmatrix},\\
&\begin{pmatrix}0&1\\1&0\end{pmatrix},
\begin{pmatrix}0&\alpha\\\alpha^2&0\end{pmatrix},
\begin{pmatrix}0&\alpha^2\\\alpha&0\end{pmatrix}\bigg\}.
\end{aligned}}
$$

The [group isomorphism](../../../../group-isomorphism.md) $r\mapsto(123)$, $s\mapsto(12)$ identifies this [group](../../../../group-split.md) with the [symmetric group](../../../../symmetric-group.md) $S_3$, with [permutations](../../../../permutation.md) composed from right to left.

Conjugation by $s$ exchanges $r,r^2$. Conjugation by $r$ cycles $s,rs,r^2s$, because $r(r^ks)r^{-1}=r^{k+2}s$. Their [conjugacy classes](../../../../conjugacy-class.md) are

$$
\boxed{\{I_2\},\qquad\{r,r^2\},\qquad\{s,rs,r^2s\},}
$$

with sizes $1,2,3$. There is no mixing between them: their elements have orders one, three and two, respectively.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../c/solution.md)
