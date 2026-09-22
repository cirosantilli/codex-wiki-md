<h1 id="12f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Away from zero and the zeros of $\cos(\pi/x)$, the [sign function](../../../../../../sign-function.md) is locally constant and the [absolute value function](../../../../../../absolute-value.md) is differentiable at the value of the cosine. The [product rule](../../../../../../product-rule.md) and [chain rule](../../../../../../chain-rule.md) give

$$
\begin{aligned}
f'(x)
&=2x\operatorname{sign}(x)\left|\cos\frac\pi x\right|
+x^2\operatorname{sign}(x)\operatorname{sign}\left(\cos\frac\pi x\right)
\frac\pi{x^2}\sin\frac\pi x\\
&=2|x|\left|\cos\frac\pi x\right|
+\pi\operatorname{sign}(x)\operatorname{sign}\left(\cos\frac\pi x\right)
\sin\frac\pi x.
\end{aligned}
$$

Thus the [triangle inequality](../../../../../../triangle-inequality.md) and the bounds on [sine](../../../../../../sine.md) and [cosine](../../../../../../cosine.md) imply $|f'(x)|\leq2|x|+\pi$. Part (c) rules out differentiability at every nonzero cosine zero, and part (b) gives $f'(0)=0$, so this estimate covers every point where the [derivative](../../../../../../derivative.md) exists.

For a finite interval $I$, choose $L<\infty$ such that $|x|\leq L$ throughout $I$. Then

$$
\boxed{|f'(x)|\leq C_I:=2L+\pi\quad(x\in I\text{ where }f'(x)\text{ exists}).}
$$

The apparent $x^{-2}$ factor in the derivative of the oscillation cancels against the multiplying $x^2$, which is what makes a uniform bound possible even near zero.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
