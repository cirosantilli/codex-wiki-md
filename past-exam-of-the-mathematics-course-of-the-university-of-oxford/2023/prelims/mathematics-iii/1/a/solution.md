<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With the [change of variables](../../../../../../change-of-variables-formula.md) $z=y^2$, multiplication of the [differential equation](../../../../../../differential-equation-split.md) by $2y$ gives $z'+2xz=2x$. The [integrating factor](../../../../../../integrating-factor.md) is $e^{x^2}$, so

$$
(ze^{x^2})'=2xe^{x^2},\qquad z=1+Ce^{-x^2}.
$$

The [initial condition](../../../../../../initial-condition.md) gives $C=3$. Since $y$ starts negative and $z\geq1$, [continuity](../../../../../../continuous-function.md) selects the negative [square root](../../../../../../square-root.md) throughout:

$$
\boxed{y(x)=-\sqrt{1+3e^{-x^2}}\quad(x\in\mathbb R).}
$$

This never reaches the singular value $y=0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
