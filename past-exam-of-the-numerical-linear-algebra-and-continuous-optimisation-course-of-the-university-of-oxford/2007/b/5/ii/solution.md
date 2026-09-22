<h1 id="b/5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Cauchy point](../../../../../cauchy-point.md) minimizes the model along the negative-gradient ray within the ball. For $g\ne0$, write $s=-tg$, $0\leq t\leq\Delta/\|g\|_2$. Then

$$
m(-tg)=f(x)-t\|g\|_2^2+\frac12t^2\|g\|_2^2,
$$

whose scalar minimum occurs at $t=1$ unless the ball cuts the ray short. Therefore

$$
\boxed{s_c=-\min\{1,\Delta/\|g\|_2\}\,g.}
$$

If $\|g\|_2\leq\Delta$, its predicted decrease is $\tfrac12\|g\|_2^2$. Otherwise it is $\Delta\|g\|_2-\tfrac12\Delta^2\geq\tfrac12\Delta\|g\|_2$. Thus every feasible step with $m(s)\leq m(s_c)$ satisfies the [Cauchy decrease bound](../../../../../cauchy-decrease-bound.md)

$$
\boxed{f(x)-m(s)\geq\frac12\|g\|_2\min\{\|g\|_2,\Delta\}.}
$$

For $g=0$, take $s_c=0$; the bound reduces to zero.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
