<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Inada conditions](../../../../../../inada-conditions.md) give $U'(0+)=\infty$ and $U'(\infty)=0$. [Differentiability](../../../../../../differentiability.md) and [strict concavity](../../../../../../strict-concavity.md) make $U'$ continuous and strictly decreasing, with range $(0,\infty)$. Hence the [inverse marginal utility](../../../../../../inverse-marginal-utility.md) $I=(U')^{-1}$ exists. The unique maximizer in the [utility conjugate](../../../../../../utility-conjugate.md) is $x=I(y)$, and

$$
\widehat U(y)=U(I(y))-yI(y),\qquad\boxed{\widehat U'(y)=-I(y).}
$$

The [derivative](../../../../../../derivative.md) formula does not require [differentiability](../../../../../../differentiability.md) of $I$: compare the optimizing values at $y$ and $y+h$ to squeeze the [difference quotient](../../../../../../difference-quotient.md) between $-I(y)$ and $-I(y+h)$, and use [continuity](../../../../../../continuous-function.md) of $I$. Thus the dual is continuously differentiable, strictly decreasing, and [strictly convex](../../../../../../strictly-convex-function.md), since $-I$ is strictly increasing.

For the requested second-derivative assertion, a curvature hypothesis is missing. Under the intended nondegeneracy $U''(x)<0$ for every $x>0$, inverse differentiation gives

$$
\boxed{\widehat U''(y)=-\frac1{U''(I(y))}>0,\qquad U''(x)\widehat U''(U'(x))=-1.}
$$

This proves the intended [dual differentiability with nonvanishing utility curvature](../../../../../../dual-differentiability-with-nonvanishing-utility-curvature.md). If $U$ is only twice differentiable, it gives pointwise twice [differentiability](../../../../../../differentiability.md) of the dual; continuous second [derivatives](../../../../../../derivative.md) additionally follow when $U\in C^2$.

Literal [strict concavity](../../../../../../strict-concavity.md) does not imply nonvanishing curvature. An explicit [Inada utility with vanishing curvature](../../../../../../inada-utility-with-vanishing-curvature.md) is

$$
U(x)=\log x+\frac1x-\frac1{6x^2},\quad U'(x)=\frac1x-\frac1{x^2}+\frac1{3x^3},\quad U''(x)=-\frac{(x-1)^2}{x^4}.
$$

Its [derivative](../../../../../../derivative.md) is positive, strictly decreasing, tends to infinity at zero and to zero at infinity. It is smooth and [strictly concave](../../../../../../strictly-concave-function.md), but $U''(1)=0$. At $y_0=U'(1)=1/3$, a finite [derivative](../../../../../../derivative.md) of $I$ would contradict differentiation of $U'(I(y))=y$, giving $0\cdot I'(y_0)=1$. Hence $\widehat U'$ is not differentiable there. **As printed, the twice-differentiable-dual claim is false; it is valid with $U''<0$.** The remaining [differentiability](../../../../../../differentiability.md), monotonicity and strict-convexity conclusions above hold under the printed hypotheses.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
