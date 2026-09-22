<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $f>0$ set $\tau=ft$ and $y(\tau)=p_0(t)$. The [master equation](../../../../master-equation.md) becomes

$$
y'=-y+2p_B,\qquad p_A'=y-p_A+p_B,\qquad p_B'=p_A-3p_B.
$$

Using $p_A=1-y-p_B$ and $p_B=(y'+y)/2$ gives

$$
y''+5y'+6y=2.
$$

Initially the molecule occupies $B$, so $y(0)=0$ and $y'(0)=2$. The characteristic roots are $-2,-3$; the constant particular solution is $1/3$. Consequently

$$
y=\frac13+Ce^{-2\tau}+De^{-3\tau},\qquad C+D=-\frac13,\quad -2C-3D=2,
$$

whence

$$
\boxed{p(t)=\frac13+e^{-2ft}-\frac43e^{-3ft}.}
$$

It has the required initial slope $2f$, tends to the stationary uncharged [probability](../../../../probability.md) $1/3$, and remains nonnegative. As a further check, $p_B=1/6-e^{-2ft}/2+4e^{-3ft}/3$ and $p_A=1/2-e^{-2ft}/2$ are nonnegative and sum with $p(t)$ to one. If $f=0$, no jump occurs and $p(t)=0$, also obtained directly from the boxed expression.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
