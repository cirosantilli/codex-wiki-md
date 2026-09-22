<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the exact [line searches](../../../../line-search.md) from part (i). After minimizing along one coordinate, the corresponding [gradient](../../../../gradient.md) component is zero. Unless the optimum has been reached, the whole nonzero [gradient](../../../../gradient.md) therefore lies along the other coordinate, which is selected next. The chosen signed coordinate direction then has $\cos\theta_k=1$. A selected zero [gradient](../../../../gradient.md) component can be skipped; it already minimizes that coordinate.

The [Zoutendijk theorem](../../../../zoutendijk-theorem.md) therefore gives $\nabla f(x_k)\to0$. The unique point with zero [gradient](../../../../gradient.md) is

$$
\boxed{x^*=\left(\frac{a+b}{2},\frac{a-b}{2}\right),\qquad f(x^*)=0.}
$$

Since $\nabla f(x)=H(x-x^*)$ and $H$ is invertible, [gradient](../../../../gradient.md) [convergence](../../../../convergence.md) implies $x_k\to x^*$. Positive definiteness makes this the unique [global minimum](../../../../global-minimum.md).

[Convergence](../../../../convergence.md) also holds if “[line search](../../../../line-search.md)” is interpreted as any fixed-parameter [Wolfe search](../../../../wolfe-conditions.md). If coordinate $i$ is selected, its signed step $s$ satisfies $s=-\omega g_i/h$, where $h=c^{-2}+d^{-2}$ and $1-\eta\leq\omega\leq2(1-\sigma)$. Sufficient decrease gives $f(x_k)-f(x_{k+1})\geq\sigma(1-\eta)g_i(x_k)^2/h$. Summation shows that selected [gradient](../../../../gradient.md) components tend to zero and step lengths tend to zero. The other component was selected in the preceding step; [Lipschitz continuity](../../../../lipschitz-continuity.md) then makes it tend to zero as well. Thus the full [gradient](../../../../gradient.md) converges to zero. The simple one-step angle argument and sharp Q-linear factor below use exact coordinate minimization; arbitrary Wolfe choices need not have that same Euclidean one-step factor.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
