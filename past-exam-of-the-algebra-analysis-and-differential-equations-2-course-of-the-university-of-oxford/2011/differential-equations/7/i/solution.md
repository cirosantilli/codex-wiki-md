<h1 id="differential-equations/7/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First prove the general uniqueness claim. The bound $Mh\leq k$ prevents a solution from leaving the dependent-variable interval before $|x-a|=h$: up to any first exit, $|y(x)-b|\leq M|x-a|\leq k$. Let $y_1,y_2$ be two solutions with the same initial value. Their integral equations and the [Lipschitz condition](../../../../../lipschitz-continuity.md) give, for $x\geq a$,

$$
|y_1(x)-y_2(x)|\leq A\int_a^x|y_1(s)-y_2(s)|\,ds.
$$

Since their difference is bounded by $2k$, repeated substitution into this inequality proves, for every integer $n\geq0$,

$$
|y_1(x)-y_2(x)|\leq2k\frac{(A|x-a|)^n}{n!}.
$$

The same argument with reversed limits works for $x\leq a$. Letting $n\to\infty$ forces the difference to zero on the whole interval. This proves at most one solution without assuming that $Ah<1$.

For case (i), choose a rectangle around $(0,1)$ that stays in $y>0$. There $f_y=(2/3)xy^{-1/3}$ is bounded, giving a uniform Lipschitz constant by the mean value theorem. For example $h=k=1/2$ works: $M\leq\tfrac12(3/2)^{2/3}$ and $Mh<1/2$. Separate variables using $u=y^{1/3}$, obtaining $3u'=x$. The initial condition gives $u=1+x^2/6$, hence

$$
\boxed{y(x)=\left(1+\frac{x^2}{6}\right)^3.}
$$

It remains positive for all real $x$, so the same local uniqueness argument continues along this solution.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [7](../../7.md)
3. [Differential Equations](../../../differential-equations.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
