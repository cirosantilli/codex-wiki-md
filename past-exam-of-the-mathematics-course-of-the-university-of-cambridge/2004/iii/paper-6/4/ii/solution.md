<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $F$ is empty, the zero [linear functional](../../../../../../linear-functional.md) satisfies the conclusion vacuously. Otherwise choose one $f_0\in F$, put $\delta=\epsilon/2$, and form the [convex set](../../../../../../convex-set.md)

$$
E=F+B(0,\delta)-f_0.
$$

It contains $B(0,\delta)$ because $f_0\in F$. The point $x=-f_0$ is outside $E$: membership would imply $0=f+u$ for some $f\in F$ with $\|u\|<\delta$, contradicting the assumed absence of points of $F$ in $B(0,\epsilon)$.

Apply part (i). There is a [continuous linear functional](../../../../../../continuous-linear-functional.md) $T$ with $T(-f_0)\geq1$ and $T(f+u-f_0)\leq1$ for every $f\in F$, $\|u\|<\delta$. Thus $T\ne0$ and

$$
Tf+Tu\leq1+Tf_0\leq0.
$$

For fixed $f$, take the supremum of $Tu$ over this [open ball](../../../../../../open-ball.md); it is $\delta\|T\|$. Consequently $Tf\leq-\delta\|T\|$ for every $f\in F$. The normalization

$$
\boxed{S=-\frac{T}{\delta\|T\|}}
$$

is a [continuous linear functional](../../../../../../continuous-linear-functional.md) satisfying $Sf\geq1$ for every $f\in F$. No [compactness](../../../../../../compact-space.md), closedness or attainment of the supremum on the [open ball](../../../../../../open-ball.md) is needed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
