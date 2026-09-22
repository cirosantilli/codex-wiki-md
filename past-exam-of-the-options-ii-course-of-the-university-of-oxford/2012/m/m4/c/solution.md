<h1 id="m/m4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume [convergence in probability](../../../../../convergence-in-probability.md) and fix $\varepsilon>0$. On the event $|Y_n-Y|\leq\varepsilon$, $Y\leq x-\varepsilon$ implies $Y_n\leq x$, while $Y_n\leq x$ implies $Y\leq x+\varepsilon$. Hence

$$
F_Y(x-\varepsilon)-\mathbb P(|Y_n-Y|>\varepsilon)
\leq F_{Y_n}(x)
\leq F_Y(x+\varepsilon)+\mathbb P(|Y_n-Y|>\varepsilon).
$$

Taking lower and upper limits in $n$ removes the error [probabilities](../../../../../probability.md). If $x$ is a [continuity point](../../../../../continuity-point.md) of $F_Y$, letting $\varepsilon\downarrow0$ squeezes both bounds to $F_Y(x)$. Thus

$$
\boxed{Y_n\to Y\text{ in probability}\Longrightarrow Y_n\to Y\text{ in distribution}.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [M4](../../m4.md)
3. [M](../../../m.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
