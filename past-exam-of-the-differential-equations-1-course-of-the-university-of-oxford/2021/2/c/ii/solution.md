<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Continuous dependence of an ODE solution on parameters](../../../../../continuous-dependence-of-an-ode-solution-on-parameters.md) here means continuity of the map $\beta\mapsto y_\beta$ into $C([a-h,a+h])$ with its [supremum norm](../../../../../supremum-norm.md): for every $\beta_0\in I$ and $\varepsilon>0$, all sufficiently close $\beta\in I$ satisfy

$$
\sup_{|x-a|\leq h}|y_\beta(x)-y_{\beta_0}(x)|<\varepsilon.
$$

Subtract the two [integral equations](../../../../../integral-equation.md) and use the uniform [Lipschitz constant](../../../../../lipschitz-constant.md) $L$ on the rectangle. With $v(x)=|y_\beta(x)-y_\gamma(x)|$ we obtain

$$
v(x)\leq|\beta-\gamma|\,|x-a|+L\left|\int_a^x v(s)\,ds\right|.
$$

Part (i), with $c=|\beta-\gamma|$ and $A=L$, therefore proves, for $L>0$,

$$
\boxed{\|y_\beta-y_\gamma\|_\infty\leq\frac{e^{Lh}-1}{L}|\beta-\gamma|.}
$$

The case $\beta=\gamma$ follows from uniqueness or the same estimate with zero forcing. If $L=0$, the direct [integral](../../../../../integral-split.md) estimate gives $\|y_\beta-y_\gamma\|_\infty\leq h|\beta-\gamma|$. In either case the map is even [Lipschitz continuous](../../../../../lipschitz-continuity.md), and hence [continuous](../../../../../continuous-function.md), throughout $I$ in the stated [supremum norm](../../../../../supremum-norm.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
