<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a step size $\tau>0$, define the set-valued maps

$$
\boxed{F_{\tau f}=I-\tau\partial f,\qquad B_{\tau f}=(I+\tau\partial f)^{-1}.}
$$

The [forward subgradient step](../../../../../../forward-subgradient-step.md) maps $x$ to the set $\{x-\tau p:p\in\partial f(x)\}$. If $f$ is differentiable this is the explicit gradient step $x-\tau\nabla f(x)$. The [backward subgradient step](../../../../../../proximal-operator.md) consists of the $y$ satisfying $x-y\in\tau\partial f(y)$, an implicit step for the [subgradient](../../../../../../subgradient.md) flow. It is the [resolvent of a monotone operator](../../../../../../resolvent-of-a-monotone-operator.md) associated with $\partial f$.

Suppose $y_1,y_2\in B_{\tau f}(x)$. Then $p_i=(x-y_i)/\tau\in\partial f(y_i)$. The two defining [subgradient inequalities](../../../../../../subgradient-inequality.md) are

$$
f(y_2)\geq f(y_1)+\langle p_1,y_2-y_1\rangle,\qquad
f(y_1)\geq f(y_2)+\langle p_2,y_1-y_2\rangle.
$$

Their sum proves [monotonicity of a convex subdifferential](../../../../../../monotonicity-of-a-convex-subdifferential.md), $\langle p_1-p_2,y_1-y_2\rangle\geq0$. But $p_1-p_2=-(y_1-y_2)/\tau$, so

$$
0\leq-\frac1\tau\|y_1-y_2\|^2,\qquad\boxed{y_1=y_2}.
$$

Convexity supplies the [subgradient](../../../../../../subgradient.md) inequalities and monotonicity; membership in the [subdifferential](../../../../../../subdifferential.md) ensures the two function values are finite, so subtraction is legitimate. Positivity of $\tau$ supplies the decisive sign. Properness rules out the identically infinite and negative-infinity pathologies in the overall setting, but [lower semicontinuity](../../../../../../lower-semicontinuity.md) is not needed for this at-most-one argument. Its role is in existence, proved next. The backward step cannot have two values, though uniqueness alone has not yet shown its domain is all of $\mathbb R^n$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
