<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose a [line](../../../../../../../straight-line.md) $T$ through $\mathbf y$ meets each $L_i$. Its intersection with $L_i$ is different from $\mathbf y$, so $T$ lies in $\Pi_i$. A nonzero [direction vector](../../../../../../../direction-vector.md) $\mathbf d$ for $T$ must therefore satisfy

$$
M\mathbf d=\mathbf0,\qquad
M=\begin{pmatrix}
0&1-y_3&y_2\\
y_3&0&1-y_1\\
1-y_2&y_1&0
\end{pmatrix}.
$$

A square [matrix](../../../../../../../matrix.md) admitting a nonzero [vector](../../../../../../../vector.md) $\mathbf d$ with $M\mathbf d=\mathbf0$ has zero [determinant](../../../../../../../determinant.md). Expanding gives

$$
\begin{aligned}
0=\det M
&=(1-y_1)(1-y_2)(1-y_3)+y_1y_2y_3\\
&=1-y_1-y_2-y_3+y_1y_2+y_2y_3+y_3y_1.
\end{aligned}
$$

Thus the necessary condition is

$$
\boxed{y_1+y_2+y_3-y_1y_2-y_2y_3-y_3y_1=1.}
$$

**The condition is not sufficient.** Take $\mathbf y=(2,1,0)$, which is on none of the three original [lines](../../../../../../../straight-line.md). It satisfies the condition, since $2+1-2=1$. The three [plane](../../../../../../../plane.md) equations become

$$
r_2+r_3=1,\qquad -r_3=0,\qquad 2r_2=2.
$$

Their common intersection is the single [line](../../../../../../../straight-line.md) $T=\{(s,1,0):s\in\mathbb R\}$. Any proposed [line](../../../../../../../straight-line.md) through $\mathbf y$ meeting all three original [lines](../../../../../../../straight-line.md) would have to be this $T$. But $T$ never meets $L_1=\{(s,0,1):s\in\mathbb R\}$: their second and third [coordinates](../../../../../../../coordinate-linear-algebra.md) differ. The zero [determinant](../../../../../../../determinant.md) guarantees a common direction for the three [planes](../../../../../../../plane.md); it does not guarantee the required intersections. This is a [parallel obstruction to a transversal of three skew lines](../../../../../../../parallel-obstruction-to-a-transversal-of-three-skew-lines.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
