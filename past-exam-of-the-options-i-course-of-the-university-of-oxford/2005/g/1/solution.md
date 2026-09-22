<h1 id="g/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For fixed endpoint values, the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is

$$
\boxed{\frac d{dx}F_{y'}(x,y,y')-F_y(x,y,y')=0.}
$$

It follows by differentiating the functional along $y+\varepsilon\eta$ with $\eta(0)=\eta(\pi)=0$, integrating the $F_{y'}\eta'$ term by parts and applying the [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md).

For this quadratic integrand it becomes $y''+ky=0$. If $k>0$, write $\nu=\sqrt k$; the condition at zero gives $y=B\sin(\nu x)$, and that at $\pi$ requires $B\sin(\nu\pi)=0$. Consequently **$y=0$ is the only [extremal](../../../../extremal.md) when $\sqrt k$ is not an integer**. If $\sqrt k=n$ is a positive integer, all [extremals](../../../../extremal.md) are

$$
\boxed{y(x)=B\sin(nx),\qquad B\in\mathbb R.}
$$

The integer case $n=0$ must be handled separately: $y''=0$ with both endpoints zero has only $y=0$. If negative real $k$ is allowed, the hyperbolic-[function](../../../../function-split.md) solutions also yield only zero under these endpoints. These statements concern stationary [functions](../../../../function-split.md); no minimum is assumed.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [G](../../g.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
