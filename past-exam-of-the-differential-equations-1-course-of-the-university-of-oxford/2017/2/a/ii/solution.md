<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $0<\eta\leq h$, work on the closed subset

$$
C_\eta=\{y\in C([a-\eta,a+\eta]): |y(x)-b|\leq k\},\qquad d(y,z)=\|y-z\|_\infty.
$$

It is a nonempty [complete metric space](../../../../../complete-metric-space.md) because it is closed in the [Banach space](../../../../../banach-space-split.md) of continuous functions with the [supremum norm](../../../../../supremum-norm.md). Define the [Picard iteration](../../../../../picard-iteration.md) operator

$$
(Ty)(x)=b+\int_a^x f(s,y(s))\,ds.
$$

Choose $\eta$ so that **$M\eta\leq k$ and $L\eta<1$**, omitting a bound whose constant is zero. Such a positive $\eta$ exists. The first inequality makes $T$ a self-map, since $|(Ty)(x)-b|\leq M|x-a|\leq k$. The [Lipschitz condition](../../../../../lipschitz-continuity.md) gives

$$
\|Ty-Tz\|_\infty\leq L\eta\|y-z\|_\infty,
$$

so the [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) yields a unique fixed point. The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) makes it a differentiable solution of $y'=f(x,y)$ with $y(a)=b$; conversely every solution staying in the rectangle satisfies the integral equation and is a fixed point. This is the local [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md) construction. The interval-restricted space $C_\eta$ avoids treating functions defined on a shorter interval as elements of $C_h$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
