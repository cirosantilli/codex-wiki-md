<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove the required [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) directly. Fix $t_0>0$, and take a compact parameter [interval](../../../../../interval-mathematics.md) $J\subseteq[0,\infty)$ containing $t_0$ in its interior. The jointly continuous [partial derivative](../../../../../partial-derivative.md) $\partial_t f$ is bounded on the compact rectangle $J\times[0,1]$ by some $M_1$.

For nonzero $h$ sufficiently close to zero, define

$$
D_h(x)=\frac{f(t_0+h,x)-f(t_0,x)}h.
$$

For each $x$, the [mean value theorem](../../../../../mean-value-theorem.md) in the parameter gives $|D_h(x)|\leq M_1$. The definition of the [partial derivative](../../../../../partial-derivative.md) also gives $D_h(x)\to\partial_t f(t_0,x)$. Since $M_1$ is integrable on $[0,1]$, [dominated convergence](../../../../../dominated-convergence-theorem.md) applied along any sequence $h_n\to0$ yields

$$
\lim_{h\to0}\frac{F(t_0+h)-F(t_0)}h
=\lim_{h\to0}\int_0^1D_h(x)\,dx
=\int_0^1\partial_t f(t_0,x)\,dx.
$$

Thus

$$
\boxed{F'(t)=\int_0^1\frac{\partial f(t,x)}{\partial t}\,dx\qquad(t>0).}
$$

At $t=0$, repeat the argument on $J=[0,\delta]$ with $h>0$. It proves that the [right derivative](../../../../../right-derivative.md) exists and satisfies the same formula at zero. This is the appropriate meaning of differentiability on the closed half-line. In fact $F'$ is continuous there: apply part (i) to the continuous [function](../../../../../function-split.md) $\partial_t f$.

The proof establishes [differentiation of parameter integrals on compact rectangles](../../../../../differentiation-of-parameter-integrals-on-compact-rectangles.md) under the exact regularity assumptions used here. In particular, it supplies the theorem's proof instead of assuming an interchange of a [limit](../../../../../limit-of-a-function.md) and an [integral](../../../../../integral-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
