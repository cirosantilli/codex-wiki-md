<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep all four [relators](../../../../../../relator.md) and all five generators, in the orders $(r_A,r_B,r_C,r_D)$ and $(d,e,a,b,c)$. Under [abelianization](../../../../../../abelianization.md), these generators become $(t,t,t^2,t^3,t^2)$. The [Fox calculus](../../../../../../fox-calculus.md) rules are

$$
\frac{\partial(uv)}{\partial x}=\frac{\partial u}{\partial x}+u\frac{\partial v}{\partial x},\qquad
\frac{\partial x^{-1}}{\partial x}=-x^{-1}.
$$

For example, $r_B=ad^{-1}cb^{-1}$ gives the nonzero [Fox derivative](../../../../../../fox-derivative.md) entries $-ad^{-1}$, $1$, $-ad^{-1}cb^{-1}$, $ad^{-1}$ in columns $d,a,b,c$, respectively. After [abelianization](../../../../../../abelianization.md) these are $-t,1,-1,t$. The full [Alexander matrix](../../../../../../alexander-matrix.md) is

$$
\boxed{A=\begin{pmatrix}
-1&-t&1&0&0\\
-t&0&1&-1&t\\
0&t&-t&1&-1\\
-t&-1&0&0&1
\end{pmatrix}.}
$$

The [Fox calculus](../../../../../../fox-calculus.md) identity supplies a useful check:

$$
A\begin{pmatrix}t-1\\t-1\\t^2-1\\t^3-1\\t^2-1\end{pmatrix}=0.
$$

Deleting the $e$ column, adjacent to the unbounded region across the marked [meridian of a knot](../../../../../../meridian-of-a-knot.md), gives

$$
B=\begin{pmatrix}-1&1&0&0\\-t&1&-1&t\\0&-t&1&-1\\-t&0&0&1\end{pmatrix},\qquad
\det B=-t^2+3t-1.
$$

Thus $\det B$ is a representative of the [Alexander polynomial of a knot](../../../../../../alexander-polynomial.md) of the [figure-eight knot](../../../../../../figure-eight-knot.md), with its customary ambiguity of multiplication by $\pm t^n$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 141](../../../paper-141-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
