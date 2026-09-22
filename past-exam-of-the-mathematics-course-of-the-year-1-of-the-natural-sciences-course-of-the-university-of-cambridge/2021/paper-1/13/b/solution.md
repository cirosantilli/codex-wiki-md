<h1 id="13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First retain the equilibrium solution $\boxed{y\equiv0}$. Any nonzero real solution has constant sign on its interval of existence, since the polynomial right-hand side is [locally Lipschitz](../../../../../locally-lipschitz-function.md) and [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md) prevents crossing the zero solution.

For a nonzero solution, the [Bernoulli differential equation](../../../../../bernoulli-differential-equation.md) substitution $u=y^{-4}$ gives

$$
u'=-4y^{-5}y'=-8u-16.
$$

This [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) has solution $u+2=Ce^{-8x}$. Therefore every nonzero real solution is

$$
\boxed{y(x)=\pm\bigl(Ce^{-8x}-2\bigr)^{-1/4},\qquad C>0,\quad x<\frac18\ln\frac C2.}
$$

Either sign may be chosen and remains fixed. The restriction ensures $y^{-4}>0$; nonpositive $C$ gives no nonzero real solution. These are maximal real intervals, and their restrictions are also solutions. As the right endpoint is approached, $|y|$ diverges in [finite-time blowup](../../../../../finite-time-blowup.md). The substitution would have lost $y=0$ if it had not been checked separately.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
