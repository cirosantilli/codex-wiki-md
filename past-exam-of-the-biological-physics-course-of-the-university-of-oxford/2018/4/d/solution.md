<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use Y and Z as the variables appearing in the equations; the introductory reference to X and Y is a naming mismatch. With $\gamma>0$, $n>0$, a symmetric [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) has $Y=Z=x$ and

$$
\boxed{x(1+x^n)=\gamma.}
$$

The left side increases continuously from zero to infinity because its [derivative](../../../../derivative.md) is $1+(n+1)x^n>0$. Thus there is exactly one positive symmetric solution for every allowed parameter pair, which verifies the implicit steady-state expression.

For $\gamma\gg1$ and $n\gg1$, look for one high component and one low component. If $Y\sim\gamma$, the other equation gives $Z=\gamma/(1+Y^n)\sim\gamma^{1-n}\ll1$; that small value in turn gives $Y=\gamma/(1+Z^n)\sim\gamma$. Exchanging the components gives the alternative state:

$$
\boxed{(Y,Z)\sim(\gamma,\gamma^{1-n})
\quad\text{and}\quad(\gamma^{1-n},\gamma).}
$$

For example the relative correction to the high value is of order $\gamma^{-n(n-1)}$, while the low value first has the ordinary denominator correction of relative order $\gamma^{-n}$. The sharply repressive [Hill function](../../../../hill-function.md) is therefore consistent with two alternatives, one factor high and the other low, which can encode a switch. [Mutual repression](../../../../mutual-repression.md) makes a [positive feedback](../../../../positive-feedback.md) loop: a high Y suppresses Z and thereby relieves repression of Y. Existence of alternative equilibria alone does not establish their [stability](../../../../stability-of-a-numerical-method.md); the explicit quadratic-Hill case in part (e) also permits that check.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
