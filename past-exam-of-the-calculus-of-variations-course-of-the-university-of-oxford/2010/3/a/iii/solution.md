<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The finite-energy comparison $I_\varepsilon(u_\varepsilon)\leq I_\varepsilon(x)<\infty$ gives $\varepsilon\int|u_\varepsilon'|^{4/3}<\infty$. Together with the endpoint value and [absolute continuity](../../../../../absolutely-continuous-function.md), this proves $u_\varepsilon\in W^{1,4/3}(0,1)$.

For $\alpha>1/4$, the power competitor $u_\alpha=x^\alpha$ is admissible and has finite [derivative](../../../../../derivative.md) energy. Direct integration gives

$$
I_\varepsilon(u_\alpha)=\frac1{8\alpha+1}-\frac2{4\alpha+2}+\frac13+\frac{3\varepsilon\alpha^{4/3}}{4\alpha-1}.
$$

Choose $\delta=\varepsilon^{1/3}$ and $\alpha=1/4+\delta$. The first three terms tend to zero as $\alpha\downarrow1/4$, while the last equals $\tfrac34\varepsilon^{2/3}(1/4+\varepsilon^{1/3})^{4/3}\to0$. By minimality and nonnegativity,

$$
\boxed{0\leq I_\varepsilon(u_\varepsilon)\leq I_\varepsilon(u_{1/4+\varepsilon^{1/3}})\longrightarrow0.}
$$

One also obtains the quantitative bound $I_\varepsilon(u_\varepsilon)=O(\varepsilon^{2/3})$: for $\alpha=1/4+\delta$, the [mean value theorem](../../../../../mean-value-theorem.md) gives $|x^{4\alpha}-x|\leq4\delta x|\log x|$, and $\int_0^1x^2\log^2x\,dx=2/27$. Thus the squared mismatch is at most $32\delta^2/27$, matching the order of the [derivative](../../../../../derivative.md) penalty with this choice. This is a [power-law comparison for vanishing derivative regularization](../../../../../power-law-comparison-for-vanishing-derivative-regularization.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the calculus of variations course of the University of Oxford](../../../../split.md)
6. [Calculus of variations course of the University of Oxford](../../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
