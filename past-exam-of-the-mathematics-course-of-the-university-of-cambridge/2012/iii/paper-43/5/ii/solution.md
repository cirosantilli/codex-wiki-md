<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For [secant domination for expected utility derivatives](../../../../../../secant-domination-for-expected-utility-derivatives.md), at each sample value $x$ set $g_x(\theta)=U(\theta x)$. This is a differentiable concave function, regardless of the sign of $x$. Fix $\theta_0$ and $\delta>0$. For $\theta\in[\theta_0-\delta,\theta_0+\delta]$, concavity bounds its derivative between the two outer secant slopes:

$$
\frac{g_x(\theta_0+2\delta)-g_x(\theta_0+\delta)}\delta\leq g'_x(\theta)\leq\frac{g_x(\theta_0-\delta)-g_x(\theta_0-2\delta)}\delta.
$$

Because $U<0$, finiteness of $F$ means $\mathbb E|U(\eta X)|<\infty$ at each of these four endpoints. Their absolute values divided by $\delta$ therefore give a common integrable bound on $|g'_X(\theta)|$. Difference quotients satisfy the same bound by the [mean value theorem](../../../../../../mean-value-theorem.md). The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) permits differentiation under the [expectation](../../../../../../expected-value.md), and pointwise continuity of $XU'(\theta X)$ with the same bound gives continuity of the derivative. **Hence $\boxed{F'(\theta)=\mathbb E[XU'(\theta X)]}$ and $F\in C^1(\mathbb R)$.** This argument proves absolute [integrability](../../../../../../integrability.md) of the displayed derivative; no unjustified differentiation assumption is needed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
