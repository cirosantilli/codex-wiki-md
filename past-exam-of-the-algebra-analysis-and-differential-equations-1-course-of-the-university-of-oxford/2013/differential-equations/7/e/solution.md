<h1 id="differential-equations/7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The quantitative [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md) applies on a rectangle $|x-x_0|\leq a$, $\|Z-B\|_\infty\leq b$. Suppose $F$ is continuous there, bounded in [maximum norm](../../../../../supremum-norm.md) by $M$, and uniformly [Lipschitz continuous](../../../../../lipschitz-continuity.md) in $Z$. Then the [initial value problem](../../../../../initial-value-problem.md) $Y'=F(x,Y)$, $Y(x_0)=B$, has a unique solution on

$$
\boxed{|x-x_0|\leq h,\qquad h=\min\{a,b/M\},}
$$

with the usual interpretation $b/M=\infty$ if $M=0$. The solution remains in the dependent-variable ball. Its endpoints are included when $F$ is continuous on the closed rectangle, as here. Equivalently, existence first on every smaller interval and the derivative bound give extension to those endpoints.

For the given cube, $x_0=0$ and $a=b=1$. Thus the theorem gives $h=\min\{1,1/M\}$ once a bound $M$ and a uniform [Lipschitz constant](../../../../../lipschitz-constant.md) have been established. The theorem does not require $Lh<1$: convergence of [Picard iteration](../../../../../picard-iteration.md) can be proved by factorial estimates or by using successive shorter intervals.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [7](../../7.md)
3. [Differential Equations](../../../differential-equations.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
