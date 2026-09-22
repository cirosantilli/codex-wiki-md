<h1 id="differential-equations/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

[Continuity](../../../../continuous-function.md) on the [compact](../../../../compact-space.md) rectangle gives finite constants $M=\max_R|F|$ and $L=\max_R|F_y|$. The real [mean value theorem](../../../../mean-value-theorem.md) in the second coordinate gives $|F(x,y)-F(x,z)|\le L|y-z|$ within the rectangle. Define the [Picard iterates](../../../../picard-iterate.md) on the entire interval by

$$
y_0(x)=b,\qquad y_{n+1}(x)=b+\int_a^xF(t,y_n(t))dt.
$$

If the previous iterate stays in the vertical range of $R$, then $|y_{n+1}(x)-b|\le M|x-a|\le Mh\le k$. Induction therefore makes all these iterates well defined on $|x-a|\le h$.

Repeated use of the [Lipschitz bound](../../../../lipschitz-bound.md) gives the factorial estimate

$$
|y_{n+1}(x)-y_n(x)|\le\frac{ML^n|x-a|^{n+1}}{(n+1)!}\quad(n\ge0).
$$

The case $n=0$ is the direct integral bound; integrating the estimate for $n-1$ proves the next one, on either side of $a$. The series of uniform bounds converges, so the iterates converge uniformly to a [continuous function](../../../../continuous-function.md) $y$ taking values within the closed vertical range. The Lipschitz estimate permits passage through the integral to give $y(x)=b+\int_a^xF(t,y(t))dt$. The [fundamental theorem of calculus](../../../../fundamental-theorem-of-calculus.md) now gives $y'=F(x,y)$ and $y(a)=b$. Thus the solution exists on the full stated interval; no extra restriction $Lh<1$ was used.

For the specified equation take $k=1/4$, so $3/4\le y\le5/4$. On $|x|\le h$,

$$
M=\frac{3h^2}{4(3/4)^3}=\frac{16h^2}{9}.
$$

The condition $Mh\le k$ holds at $h^3=9/64$, namely $\boxed{h=3^{2/3}/4}$. The rectangle avoids $y=0$, so both [continuity](../../../../continuous-function.md) hypotheses hold there.

Direct separation gives $4y^3y'=3x^2$, hence $(y^4)'=(x^3)'$ and the initial value yields $y^4=1+x^3$. The branch through $y(0)=1$ is

$$
\boxed{y(x)=(1+x^3)^{1/4}\quad(x>-1).}
$$

It remains positive on this interval. At $x=-1$ it reaches zero, where the differential equation is undefined, so this is its maximal real interval containing zero. The rectangle theorem supplies a sufficient interval, smaller than that actual interval.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Differential equations](../../differential-equations.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
