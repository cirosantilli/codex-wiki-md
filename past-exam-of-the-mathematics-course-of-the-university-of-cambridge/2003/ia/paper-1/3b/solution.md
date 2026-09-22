<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

A real [function](../../../../../function-split.md) is [differentiable](../../../../../differentiable-function.md) at an interior point $x$ when the finite [limit](../../../../../limit-of-a-function.md)

$$
f'(x)=\lim_{h\to0,\ h\ne0}\frac{f(x+h)-f(x)}h
$$

exists, with $h$ restricted so $x+h$ lies in its domain. In quantified form, for every $\varepsilon>0$ there is $\delta>0$ such that $0<|h|<\delta$ implies that the [difference quotient](../../../../../difference-quotient.md) differs from $f'(x)$ by less than $\varepsilon$.

To prove [differentiability implies continuity](../../../../../differentiability-implies-continuity.md), the convergent [difference quotient](../../../../../difference-quotient.md) is bounded by $|f'(x)|+1$ for sufficiently small nonzero $h$. Thus $|f(x+h)-f(x)|\le(|f'(x)|+1)|h|\to0$. This is exactly [continuity](../../../../../continuous-function.md) at $x$.

At zero, the particular function has [difference quotient](../../../../../difference-quotient.md) $h\sin(1/h)$. The bound $|h\sin(1/h)|\le|h|$ and the [squeeze theorem](../../../../../squeeze-theorem.md) give

$$
\boxed{f'(0)=0.}
$$

For $x\ne0$, the [product rule](../../../../../product-rule.md) and [chain rule](../../../../../chain-rule.md) give

$$
f'(x)=2x\sin(1/x)-\cos(1/x).
$$

At $x_k=1/(2\pi k)$ this equals $-1$, although $x_k\to0$ and $f'(0)=0$. At $y_k=1/((2k+1)\pi)$ it equals $+1$. Hence the derivative has no limit at zero and is **not continuous there**. This demonstrates that [differentiability does not imply continuity of the derivative](../../../../../differentiability-does-not-imply-continuity-of-the-derivative.md), even though the function itself is continuous.

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
