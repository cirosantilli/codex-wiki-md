<h1 id="17b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With $q=p'$ and $r=0$, the equation is

$$
y''''+(py')'=\lambda y.
$$

Multiply by the real [eigenfunction](../../../../../../eigenfunction.md) $y$ and integrate over $[a,b]$. The [clamped boundary conditions](../../../../../../clamped-boundary-condition.md) $y=y'=0$ at both endpoints eliminate all boundary terms, so

$$
\lambda\int_a^b y^2dx
=\int_a^b(y'')^2dx-\int_a^b p(x)(y')^2dx.
$$

Since $p(x)<0$, the right side is a sum of nonnegative terms. It cannot vanish for a nonzero eigenfunction: if $y''=y'=0$, the boundary conditions force $y=0$. Thus

$$
\boxed{\lambda
=\frac{\int_a^b\{(y'')^2-p(y')^2\}\,dx}{\int_a^b y^2dx}>0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17B](../../17b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
