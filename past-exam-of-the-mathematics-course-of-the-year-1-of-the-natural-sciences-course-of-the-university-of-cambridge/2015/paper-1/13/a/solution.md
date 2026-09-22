<h1 id="13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $T=t+a>0$. The [similarity solution](../../../../../similarity-solution.md) uses $y=(x+b)T^{-1/2}$, whose [partial derivatives](../../../../../partial-derivative.md) at fixed $x$ or $t$ are

$$
y_x=T^{-1/2},\qquad y_t=-\frac y{2T}.
$$

Apply the [multivariable chain rule](../../../../../multivariable-chain-rule.md) to $u=T^{-1/2}v(y)$:

$$
u_t=-\frac12T^{-3/2}v+T^{-1/2}v'\left(-\frac y{2T}\right)
=-\frac12T^{-3/2}(v+yv'),
$$



$$
u_x=T^{-1}v',\qquad u_{xx}=T^{-3/2}v''.
$$

Substituting in the [heat equation](../../../../../heat-equation.md) and cancelling the positive common factor $T^{-3/2}$ gives

$$
\boxed{-\frac12(v+yv')=\lambda v''.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
