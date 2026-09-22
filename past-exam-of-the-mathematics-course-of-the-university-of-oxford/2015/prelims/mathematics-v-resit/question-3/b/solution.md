<h1 id="question-3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The original [double integral](../../../../../../double-integral.md) covers the [triangle](../../../../../../triangle.md) $0\leq y\leq x\leq1$. By [Fubini's theorem](../../../../../../fubini-s-theorem.md), after reversing the order, $y$ runs from $0$ to $1$ and $x$ from $y$ to $1$. Since a [continuous function](../../../../../../continuous-function.md) is integrable on this bounded region,

$$
\int_0^1\int_0^x f(y)\,dy\,dx
=\int_0^1\int_y^1 f(y)\,dx\,dy
=\boxed{\int_0^1(1-y)f(y)\,dy}.
$$

For the [square pyramid](../../../../../../square-pyramid.md), a horizontal section at height $z$ is a [square](../../../../../../square.md) of side $2(1-z)$: each vertex moves linearly from the base towards $(1,1,1)$. Hence its [cross-sectional area](../../../../../../cross-sectional-area.md) is $4(1-z)^2$, and its [volume](../../../../../../volume.md) is $4\int_0^1(1-z)^2\,dz$. To use the identity just proved, choose $f(y)=1-y$:

$$
\begin{aligned}
\operatorname{Vol}
&=4\int_0^1\int_0^x(1-y)\,dy\,dx\\
&=4\int_0^1\left(x-\frac{x^2}{2}\right)dx
=4\left(\frac12-\frac16\right)
=\boxed{\frac43}.
\end{aligned}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Question 3](../../question-3.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
