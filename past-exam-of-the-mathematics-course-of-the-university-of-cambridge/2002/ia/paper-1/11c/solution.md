<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

The [mean value theorem](../../../../../mean-value-theorem.md) states that, if $f$ is [continuous](../../../../../continuous-function.md) on $[a,b]$ and [differentiable](../../../../../differentiable-function.md) on $(a,b)$, with $a<b$, there is $c\in(a,b)$ such that

$$
f'(c)=\frac{f(b)-f(a)}{b-a}.
$$

To deduce it from [Rolle's theorem](../../../../../rolle-theorem.md), subtract the secant line: $k(t)=f(t)-f(a)-\frac{f(b)-f(a)}{b-a}(t-a)$. This [function](../../../../../function-split.md) has the same [continuity](../../../../../continuous-function.md) and [differentiability](../../../../../differentiability.md) properties and satisfies $k(a)=k(b)=0$. [Rolle's theorem](../../../../../rolle-theorem.md) gives an interior point with $k'(c)=0$, which is precisely the required equality.

If $h'=0$ on $\mathbb R$, apply the [mean value theorem](../../../../../mean-value-theorem.md) on any $[x,y]$ with $x<y$. It gives $h(y)-h(x)=(y-x)h'(c)=0$. Hence **$h$ is constant**.

For the [differential equation](../../../../../differential-equation-split.md), the [product rule](../../../../../product-rule.md) gives

$$
\frac{d}{dx}\bigl(e^{-ax}f(x)\bigr)=e^{-ax}\bigl(f'(x)-af(x)\bigr)=0.
$$

The preceding result makes this product constant. Thus **all solutions are $f(x)=Ce^{ax}$**, and differentiation verifies every such solution.

For the [integral](../../../../../integral.md) assertion, [continuity](../../../../../continuous-function.md) ensures that $f$ is [Riemann integrable](../../../../../riemann-integrable-function.md) on every finite [closed interval](../../../../../closed-real-interval.md). Use the usual orientation for an [integral](../../../../../integral.md) with negative upper endpoint. For $h\ne0$, additivity of the [integral](../../../../../integral.md) gives

$$
\frac{F(x+h)-F(x)}h-f(x)
=\frac1h\int_x^{x+h}\bigl(f(t)-f(x)\bigr)\,dt.
$$

The [absolute value](../../../../../absolute-value.md) of this expression is at most the [supremum](../../../../../supremum.md) of $|f(t)-f(x)|$ on the segment joining $x$ and $x+h$. [Continuity](../../../../../continuous-function.md) at $x$ makes this bound tend to zero for either sign of $h$. Consequently **$F'(x)=f(x)$**, proving this form of the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md).

Finally, a [differentiable](../../../../../differentiable-function.md) solution of the [integral equation](../../../../../integral-equation.md) is [continuous](../../../../../continuous-function.md), so the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) yields $g'=g$; setting $x=0$ gives $g(0)=A$. The differential-equation calculation above now forces

$$
\boxed{g(x)=Ae^x.}
$$

Conversely, $A+\int_0^xAe^t\,dt=A+A(e^x-1)=Ae^x$, so this [function](../../../../../function-split.md) satisfies the original [integral equation](../../../../../integral-equation.md). It is unique because every [differentiable](../../../../../differentiable-function.md) solution has already been forced to this form and this [initial condition](../../../../../initial-condition.md).

## ↑ Ancestors (11)

1. [11C](../11c.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ia](../../split.md)
5. [2002](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
