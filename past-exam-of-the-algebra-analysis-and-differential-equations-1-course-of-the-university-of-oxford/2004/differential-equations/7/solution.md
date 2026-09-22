<h1 id="differential-equations/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The first iterate is

$$
\boxed{y_1(x)=1+2x+\frac{x^3}{3}.}
$$

On the prescribed box, $F(x,y)=1+x^2+y^2$ is continuous, $|F|\leq102$, and $|F(x,y)-F(x,v)|\leq20|y-v|$. The initial value is distance nine from the nearer horizontal edge. Thus on $|x|\leq h=9/102=3/34$, the Picard map keeps functions within the box: its values differ from one by at most $102h=9$.

Successive differences satisfy, by [induction](../../../../mathematical-induction.md),

$$
|y_{n+1}(x)-y_n(x)|\leq102\frac{20^n|x|^{n+1}}{(n+1)!}.
$$

The [Weierstrass M-test](../../../../weierstrass-m-test.md) proves [uniform convergence](../../../../uniform-convergence.md) on this local interval. The [uniform limit](../../../../uniform-limit.md) is continuous, and the Lipschitz estimate allows passage to the limit inside the integral, giving the displayed integral equation. Differentiation gives $y'=1+x^2+y^2$, $y(0)=1$. The same local Lipschitz bound proves local [uniqueness](../../../../uniqueness.md).

Direct differentiation gives $u'=\sec^2(x+\pi/4)=1+u^2$, $u(0)=1$, and $u\to+\infty$ as $x\uparrow\pi/4$. On the common positive existence interval put $w=y-u$. It satisfies $w'=(y+u)w+x^2$, $w(0)=0$, so the integrating-factor formula gives

$$
w(x)=e^{\int_0^x(y+u)\,ds}\int_0^x t^2e^{-\int_0^t(y+u)\,ds}\,dt\geq0.
$$

Thus $y\geq u$. Let $x_*>0$ be the maximal forward existence endpoint. The solution is strictly increasing because $y'\geq1$. If $x_*$ were finite and $y$ remained bounded, its finite limit and the smooth right side would allow local continuation, contradicting maximality. Comparison with $u$ prevents existence through $\pi/4$. Consequently

$$
\boxed{0<x_*\leq\frac\pi4,\qquad\lim_{x\uparrow x_*}y(x)=+\infty.}
$$

There is **no contradiction with Picard's theorem**, which gives local existence and [uniqueness](../../../../uniqueness.md). Its box estimate gives only a short guaranteed interval, and the Lipschitz constant for $y^2$ is not globally bounded in $y$.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Differential equations](../../differential-equations.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
