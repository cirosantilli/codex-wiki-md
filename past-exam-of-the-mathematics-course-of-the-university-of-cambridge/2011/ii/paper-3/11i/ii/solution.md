<h1 id="11i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Since $n^{-s}-(n+1)^{-s}=s\int_n^{n+1}x^{-s-1}\,dx$, the assumed identity becomes

$$
\zeta(s)=s\int_1^\infty\lfloor x\rfloor x^{-s-1}\,dx=\frac{s}{s-1}-s\int_1^\infty\{x\}x^{-s-1}\,dx
$$

for $\operatorname{Re}s>1$, where $\{x\}$ is the [fractional part](../../../../../../fractional-part.md). Consequently

$$
\boxed{\zeta(s)-\frac1{s-1}=1-s\int_1^\infty\{x\}x^{-s-1}\,dx\qquad(\operatorname{Re}s>0).}
$$

To justify the [analytic continuation](../../../../../../analytic-continuation.md), on any compact subset of this half-plane choose $\epsilon>0$ with $\operatorname{Re}s\geq\epsilon$. The integrand is bounded by $x^{-1-\epsilon}$, an integrable function. Each derivative with respect to $s$ is bounded by a constant times $(1+\log x)^j x^{-1-\epsilon}$, also integrable. Differentiation under the integral is valid, so the right-hand side is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) throughout the half-plane, including $s=1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11I](../../11i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
