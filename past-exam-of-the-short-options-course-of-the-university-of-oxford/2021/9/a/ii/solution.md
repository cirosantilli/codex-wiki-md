<h1 id="9/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $f(N)=N[r/(1+bN^2)-\delta]$. A [steady state](../../../../../steady-state.md) is a nonnegative zero of $f$. If $r<\delta$, the bracket is strictly negative for every $N\ge0$, so only $N=0$ exists. If $r>\delta$, there are exactly two nonnegative [steady states](../../../../../steady-state.md),

$$
\boxed{N=0,\qquad N^*=\sqrt{\frac{r-\delta}{b\delta}}.}
$$

For an autonomous scalar [ordinary differential equation](../../../../../ordinary-differential-equation.md), a [steady state](../../../../../steady-state.md) with $f'<0$ is locally asymptotically stable, while one with $f'>0$ is unstable. Here

$$
f'(N)=\frac{r(1-bN^2)}{(1+bN^2)^2}-\delta,\qquad f'(0)=r-\delta.
$$

At the positive [steady state](../../../../../steady-state.md), use $1+b(N^*)^2=r/\delta$ to obtain

$$
\boxed{f'(N^*)=-\frac{2\delta(r-\delta)}r<0.}
$$

Therefore zero is **stable for $r<\delta$ and unstable for $r>\delta$**, whereas the positive [steady state](../../../../../steady-state.md) is **stable whenever it exists**. At the omitted equality $r=\delta$, $f(N)=-\delta bN^3/(1+bN^2)$; zero is nonhyperbolic but still attracts every nonnegative initial state.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
