<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here $[M]_t=t$ and $dA_t=dt$, so the formula in part (b) gives

$$
A_t^f=\int_0^t g(B_s,s)\,ds,\qquad g(x,s)=f_y(x,s)+\tfrac12f_{xx}(x,s).
$$

If $g$ vanishes on $\mathbb R\times[0,\infty)$, this integral is zero. Conversely suppose $A_t^f=0$ for all $t$ almost surely. Its integrand is continuous along each path; the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) implies $g(B_t,t)=0$ for all $t$ on that event. For any fixed $t>0$, the [normal distribution](../../../../../../normal-distribution.md) of $B_t$ has a strictly positive density at every real point. Since $g(\cdot,t)$ is continuous, a nonzero value at any spatial point would give a nonzero value on an open interval of positive Brownian probability, a contradiction. Thus $g(x,t)=0$ for every $x$ and every positive $t$. Continuity extends this to $t=0$.

Consequently the exact condition is

$$
\boxed{f_y(x,y)+\frac12f_{xx}(x,y)=0\quad\text{for every }x\in\mathbb R,\ y\geq0.}
$$

These are [space-time harmonic functions along Brownian motion](../../../../../../space-time-harmonic-functions-along-brownian-motion.md), satisfying the [backward heat equation](../../../../../../backward-heat-equation.md). The second coordinate never takes negative values, so no equation is imposed for $y<0$, beyond compatibility with the assumed global $C^2$ regularity. The normalized finite-variation term is unique by part (a), so it cannot be removed by choosing a different decomposition.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
