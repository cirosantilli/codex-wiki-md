<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the broad right layer take $\zeta=(x-1)/\sqrt\varepsilon$ and $y=Z(\zeta)$, so $\zeta\leq0$ inside the interval. Its leading equation is $Z''=\sqrt Z$, with $Z(0)=1$. One integration gives $(Z')^2=(4/3)(Z^{3/2}+c)$. The positive derivative branch produces the integral parametrization in the hint.

Matching to a small, nearly flat plateau requires $Z\to0$ and $Z'\to0$ at the inner edge, so **the leading integration constant is $c=0$**. A positive order-one $c$ would leave a nonzero slope as $Z\to0$; a negative one would prevent that limit. For $c=0$, integration with $Z(0)=1$ gives

$$
\boxed{Z(\zeta)=\left(1+\frac{\zeta}{2\sqrt3}\right)^4,\qquad -2\sqrt3\leq\zeta\leq0.}
$$

Its zero is at $\zeta=-2\sqrt3$, namely $x=1-2\sqrt{3\varepsilon}$. Near that edge it has the fourth-power overlap obtained in [solution](../b/ii/solution.md). The neglected $\varepsilon k$ reaction term becomes comparable to $\sqrt Z$ when $Z=O(\varepsilon^2)$, precisely where the thinner transition must restore it. The sketch in [solution](../solution.md) shows the plateau and both right-hand regions; extending the quartic profile past its inner edge would fail to match the positive plateau.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
