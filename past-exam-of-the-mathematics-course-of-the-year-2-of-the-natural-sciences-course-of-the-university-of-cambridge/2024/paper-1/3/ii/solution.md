<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the zero-data [initial value problem](../../../../../initial-value-problem.md), choose a [causal Green function](../../../../../causal-green-function.md) satisfying $L_xG(x,\xi)=\delta(x-\xi)$ and $G=0$ for $x<\xi$. Continuity at $x=\xi$ prevents a derivative of the [Dirac delta distribution](../../../../../dirac-delta-function.md), while integration across the source gives

$$
G(\xi^+,\xi)=0,\qquad\partial_xG(\xi^+,\xi)-\partial_xG(\xi^-,\xi)=1.
$$

For $x>\xi$, part (i) gives the shifted homogeneous solutions. The zero value at the join removes the cosine term, and the unit [derivative](../../../../../derivative.md) jump fixes the sine coefficient. Therefore the [causal Green function of a damped oscillator](../../../../../causal-green-function-of-a-damped-oscillator.md) is

$$
\boxed{G(x,\xi)=\begin{cases}\dfrac1b e^{-a(x-\xi)}\sin[b(x-\xi)],&x\geq\xi,\\0,&x<\xi.\end{cases}}
$$

Equivalently, multiply the first expression by the [Heaviside step function](../../../../../heaviside-step-function.md) $H(x-\xi)$. The required solution is

$$
\boxed{y(x)=\int_0^{\infty}G(x,\xi)g(\xi)\,d\xi=\frac1b\int_0^xe^{-a(x-\xi)}\sin[b(x-\xi)]g(\xi)\,d\xi.}
$$

Its initial value and first [derivative](../../../../../derivative.md) vanish: the interval has zero length at $x=0$ and the kernel vanishes at its upper limit. Differentiating twice shows that the upper-limit contribution to $y''$ is precisely $g(x)$, while the remaining homogeneous kernel terms cancel in $Ly$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
