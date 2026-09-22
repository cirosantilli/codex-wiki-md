<h1 id="8a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [gradient](../../../../../../gradient.md) components are

$$
f_x=y(1-2x-y),\qquad f_y=x(1-x-2y).
$$

If $x=0$ or $y=0$, their simultaneous zeros give $(0,0),(0,1),(1,0)$. If $xy\ne0$, solving $2x+y=1$, $x+2y=1$ gives $(1/3,1/3)$. These are all the [critical points](../../../../../../critical-point.md). The [Hessian matrix](../../../../../../hessian-matrix.md) is

$$
H(x,y)=\begin{pmatrix}-2y&1-2x-2y\\1-2x-2y&-2x\end{pmatrix}.
$$

At each of $(0,0),(1,0),(0,1)$ its [determinant](../../../../../../determinant.md) is $-1$, so its two [eigenvalues](../../../../../../eigenvalue.md) have opposite signs. **All three are saddle points of a scalar function.** At $(1/3,1/3)$,

$$
H=\begin{pmatrix}-2/3&-1/3\\-1/3&-2/3\end{pmatrix},
\qquad \operatorname{spec}(H)=\{-1,-1/3\}.
$$

**This point is a strict [local maximum](../../../../../../local-maximum.md), of value $\boxed{1/27}$.**

The zero [level set](../../../../../../level-set.md) is exactly

$$
\boxed{\{x=0\}\ \cup\ \{y=0\}\ \cup\ \{x+y=1\}.}
$$

These three lines form a triangle containing the maximum. Inside it $f>0$; near the maximum positive [level sets](../../../../../../level-set.md) are nested closed curves, with their leading shapes elliptical because the [Hessian matrix](../../../../../../hessian-matrix.md) is negative definite. At each vertex the zero lines cross, separating alternating signs, and nearby nonzero [level sets](../../../../../../level-set.md) have hyperbolic branches. For example, the leading quadratic terms are $xy$ at $(0,0)$, $-\eta(\xi+\eta)$ for $\xi=x-1,\eta=y$ at $(1,0)$, and $-\xi(\xi+\eta)$ for $\xi=x,\eta=y-1$ at $(0,1)$.

<a id="8a/b/image-contours-of-xy-1-x-y-showing-three-saddle-points-the-interior-maximum-and-the-three-zero-lines"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2-contours.png)

**[Figure 1](#8a/b/image-contours-of-xy-1-x-y-showing-three-saddle-points-the-interior-maximum-and-the-three-zero-lines). Contours of xy(1-x-y), showing three saddle points, the interior maximum, and the three zero lines**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8A](../../8a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
