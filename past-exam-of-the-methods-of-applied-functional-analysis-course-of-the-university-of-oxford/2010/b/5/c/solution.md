<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The displayed nonlinearity is singular at $s=-1$, so it cannot be used directly as the globally bounded function in part (b). On $s\geq0$, however,

$$
\frac12\leq f(s)=\cosh\!\left(\frac1{1+s}\right)-\frac12\sin\sqrt{1+s^2}\leq\cosh(1)+\frac12.
$$

Use [nonnegative truncation of a semilinear source](../../../../../nonnegative-truncation-of-a-semilinear-source.md): define $F(s)=f(\max\{s,0\})$. This is continuous and bounded on all of $\mathbb R$, with $F\geq1/2$. Part (b) gives a [weak solution](../../../../../weak-solution.md) of $-\Delta u=F(u)$, $u\in H_0^1$.

The [weak maximum principle](../../../../../weak-maximum-principle-for-elliptic-operators.md) in the needed form says that if $u\in H_0^1$ and $\int\nabla u\cdot\nabla\varphi\geq0$ for every nonnegative $\varphi\in H_0^1$, then $u\geq0$ [almost everywhere](../../../../../almost-everywhere.md). Here this also follows directly by testing with the negative part $u_-=\max\{-u,0\}\in H_0^1$:

$$
-\|\nabla u_-\|_2^2=\int_\Omega F(u)u_-\geq0.
$$

The [Poincaré inequality](../../../../../poincare-inequality.md) gives $u_-=0$. Hence $u\geq0$, $F(u)=f(u)$, and the denominator $1+u$ stays at least one [almost everywhere](../../../../../almost-everywhere.md). Thus **the original equation has a nonnegative weak solution**, with bounded right side.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../split.md)
6. [Methods of applied functional analysis course of the University of Oxford](../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
