<h1 id="analysis/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $t>0$, integrate $e^{itz}/(1+z^2)$ over the upper semicircle of radius $R$. The arc tends to zero, since $|e^{itz}|\le1$ there and the denominator is of order $R^2$. The sole [pole](../../../../pole.md) is $i$, of [residue](../../../../residue.md) $e^{-t}/(2i)$, so the real part gives $I(t)=\pi e^{-t}$. The integrand defining $I$ is even in $t$, and $I(0)=\pi$ by the arctangent integral. Hence

$$
\boxed{I(t)=\pi e^{-|t|}\quad(t\in\mathbb R).}
$$

For $J$ use $e^{itz}/[z(1+z^2)]$ with a small clockwise semicircular indentation above zero. Its [residue](../../../../residue.md) at zero is one, so the small arc tends to $-i\pi$. The [pole](../../../../pole.md) $i$ has [residue](../../../../residue.md) $-e^{-t}/2$, and the large arc again vanishes. Thus

$$
\operatorname{PV}\int_{-\infty}^\infty\frac{e^{itx}}{x(1+x^2)}dx-i\pi=-i\pi e^{-t}.
$$

The imaginary part is the ordinary convergent integral $J(t)$: its apparent singularity at zero is removable, with limit $t$, and its tails are absolutely integrable. Therefore $J(t)=\pi(1-e^{-t})$ for $t>0$. Oddness in $t$ and the value zero at $t=0$ give

$$
\boxed{J(t)=\begin{cases}\pi(1-e^{-t}),&t>0,\\0,&t=0,\\-\pi(1-e^{t}),&t<0.\end{cases}}
$$

[Differentiation](../../../../differentiation.md) is valid at every real $t$, including zero. Indeed the [mean value theorem](../../../../mean-value-theorem.md) bounds the absolute difference quotient of $\sin(tx)/[x(1+x^2)]$ with respect to $t$ by $1/(1+x^2)$, an integrable majorant independent of $t$. [Dominated convergence](../../../../dominated-convergence-theorem.md) therefore gives $\boxed{J'(t)=I(t)\text{ for all }t\in\mathbb R}$. In particular both one-sided derivatives at zero equal $\pi$.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Analysis](../../analysis.md)
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
