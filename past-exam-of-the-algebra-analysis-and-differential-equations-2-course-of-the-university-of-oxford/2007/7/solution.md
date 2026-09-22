<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Use [Picard iteration](../../../picard-iteration.md) on $[a-h,a+h]$:

$$
u_0(x)=b,\qquad u_{n+1}(x)=b+\int_a^x f(t,u_n(t))\,dt.
$$

By [induction](../../../mathematical-induction.md), every iterate stays in the prescribed rectangle: if $u_n$ does, then $|u_{n+1}(x)-b|\le M|x-a|\le Mh\le k$. Continuity makes each next integral well defined. The [Lipschitz condition](../../../lipschitz-continuity.md) gives, for $n\ge0$,

$$
|u_{n+1}(x)-u_n(x)|\le\frac{MA^n|x-a|^{n+1}}{(n+1)!}.
$$

For $n=0$ this is the previous bound; integration of the bound multiplied by $A$ proves the next step, on either side of $a$.

The sum of these bounds converges uniformly on the entire interval. Thus $u_n$ converges uniformly to a continuous $u$, whose graph remains in the closed rectangle. The [Lipschitz condition](../../../lipschitz-continuity.md) also makes $f(t,u_n(t))$ converge uniformly to $f(t,u(t))$, so passage to the limit gives

$$
u(x)=b+\int_a^x f(t,u(t))\,dt.
$$

The [fundamental theorem of calculus](../../../fundamental-theorem-of-calculus.md) makes $u$ a continuously differentiable solution with $u(a)=b$.

For uniqueness, let $u,v$ be two solutions and put $D_0=\sup|u-v|$ on the interval. Repeated use of the [Lipschitz condition](../../../lipschitz-continuity.md) in their integral equations gives

$$
|u(x)-v(x)|\le D_0\frac{(A|x-a|)^n}{n!}
$$

for every $n$. Letting $n\to\infty$ gives $u=v$. The global bound $M$ prevents any competing solution whose graph lies in $D$ from exiting the rectangle through a horizontal boundary before the end of the interval. Therefore **a unique solution exists on the full stated interval**. No extra restriction $Ah<1$ is needed; the factorial estimates replace that restriction.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
