<h1 id="differential-equations/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

On $[-a,a]$ let $F=\|f\|_\infty$ and bound $|K|$ by $M$ on the compact integration region. Write $Th(x)=\int_0^xK(x,s)h(s)\,ds$. The iteration gives $y_n=\sum_{j=0}^nT^jf$. Induction, integrating absolute values also when $x<0$, gives

$$
|T^jf(x)|\leq F\frac{M^j|x|^j}{j!}.
$$

The exponential series is summable uniformly for $|x|\leq a$. The [Weierstrass M-test](../../../../weierstrass-m-test.md) therefore proves [uniform convergence](../../../../uniform-convergence.md) to a [continuous function](../../../../continuous-function.md) $y$. Also $\|T(y_n-y)\|_\infty\leq Ma\|y_n-y\|_\infty\to0$, so passing to the limit yields $y=f+Ty$.

For the indicated kernel, twice differentiating its integral gives

$$
y'(x)=\int_0^x sy(s)\,ds,\qquad y''(x)=xy(x),\qquad y(0)=1,\quad y'(0)=0.
$$

Conversely integrating the differential equation twice, with these [initial conditions](../../../../initial-condition.md), gives the integral equation. This is valid also for negative $x$, either by oriented integration or by differentiating the double-integral identity.

For every finite $a$ the continuous kernel $(x-s)s$ meets the preceding hypotheses. Solutions on overlapping intervals agree: if $d=Td$ is their difference, iteration gives $\|d\|_\infty\leq\|d\|_\infty(Ma)^j/j!$ for every $j$, forcing $d=0$. The solutions therefore patch to **one solution defined on all of $\mathbb R$**.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Differential equations](../../differential-equations.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
