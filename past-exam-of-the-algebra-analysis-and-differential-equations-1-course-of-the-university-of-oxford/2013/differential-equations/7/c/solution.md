<h1 id="differential-equations/7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $a,b\geq0$ and $c\geq1$,

$$
\left|\frac1{a+c}-\frac1{b+c}\right|=\frac{|a-b|}{(a+c)(b+c)}\leq|a-b|.
$$

Apply this to the first component with $a=|z_2|$, $b=|w_2|$, $c=x^2+1$. The [reverse triangle inequality](../../../../../reverse-triangle-inequality.md) gives

$$
|F_1(x,Z)-F_1(x,W)|\leq\big||z_2|-|w_2|\big|\leq|z_2-w_2|.
$$

For the second component use $a=|z_1|$, $b=|w_1|$, $c=1$ to obtain $|F_2(x,Z)-F_2(x,W)|\leq|z_1-w_1|$. Taking the maximum yields

$$
\boxed{\|F(x,Z)-F(x,W)\|_\infty\leq\|Z-W\|_\infty.}
$$

Thus $F$ is globally [Lipschitz continuous](../../../../../lipschitz-continuity.md) in the dependent vector, uniformly in $x$, with [Lipschitz constant](../../../../../lipschitz-constant.md) $1$. Differentiability of the absolute-value function at zero is unnecessary.

## ↑ Ancestors (13)

1. [C](../c.md)
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
