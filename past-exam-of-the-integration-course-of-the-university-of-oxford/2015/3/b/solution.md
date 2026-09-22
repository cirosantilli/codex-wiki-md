<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the one-dimensional [convolution kernel](../../../../convolution-kernel.md)

$$
k(t)=\begin{cases}\sin t/|t|^{3/2},&t\ne0,\\0,&t=0.\end{cases}
$$

It is a [Borel measurable function](../../../../borel-measurable-function.md), and $f(x,y)=k(x-y)g(y)$. The [function](../../../../function-split.md) $k(x-y)$ is [Borel measurable](../../../../borel-measurable-function.md) by composition with the continuous difference map. Lifting the [Lebesgue measurable function](../../../../lebesgue-measurable-function.md) $g$ to the second coordinate preserves measurability for the [product sigma-algebra](../../../../product-sigma-algebra.md), hence also for [Lebesgue measure](../../../../lebesgue-measure.md) on $\mathbb R^2$. Products of [measurable functions](../../../../measurable-function.md) are measurable, so $f$ is [Lebesgue measurable](../../../../lebesgue-measurable-set.md).

Near zero, $|\sin t|\leq|t|$; away from zero, $|\sin t|\leq1$. Consequently

$$
|k(t)|\leq\begin{cases}|t|^{-1/2},&0<|t|\leq1,\\|t|^{-3/2},&|t|>1.\end{cases}
$$

Both bounds are integrable on their respective regions by [power singularity integrability](../../../../power-singularity-integrability.md). In particular,

$$
\boxed{\|k\|_1\leq2\int_0^1t^{-1/2}\,dt+2\int_1^\infty t^{-3/2}\,dt=4+4=8.}
$$

We use the following forms of the two product-integration theorems. On the product of [measure spaces](../../../../measure-space.md) equipped with [sigma-finite measures](../../../../sigma-finite-measure.md), [Tonelli's theorem](../../../../tonelli-theorem.md) says that a nonnegative measurable [function](../../../../function-split.md) has equal product and iterated [integrals](../../../../integral-split.md), with infinity allowed. [Fubini's theorem](../../../../fubini-s-theorem.md) says that for an absolutely integrable measurable [function](../../../../function-split.md), its sections are integrable for [almost every](../../../../almost-everywhere.md) fixed coordinate, and both orders of iterated [integration](../../../../integral-split.md) equal the finite product [integral](../../../../integral-split.md). The [Lebesgue measure](../../../../lebesgue-measure.md) on each factor is a [sigma-finite measure](../../../../sigma-finite-measure.md), because the [real line](../../../../real-line.md) is a [countable union](../../../../countable-union.md) of finite-length [intervals](../../../../interval-mathematics.md).

Apply [Tonelli's theorem](../../../../tonelli-theorem.md) first to $|f|$, before presuming finiteness. By [translation invariance of Lebesgue measure](../../../../translation-invariance-of-lebesgue-measure.md),

$$
\begin{aligned}
\int_{\mathbb R^2}|f(x,y)|\,dx\,dy
&=\int_{\mathbb R}|g(y)|\left(\int_{\mathbb R}|k(x-y)|\,dx\right)dy\\
&=\|k\|_1\int_{\mathbb R}|g(y)|\,dy
\leq8\int_{\mathbb R}|g(y)|\,dy<\infty.
\end{aligned}
$$

Thus **$f$ is [Lebesgue integrable](../../../../lebesgue-integrable-function.md) on $\mathbb R^2$**. The [triangle inequality for an integral](../../../../integral-triangle-inequality.md) now gives the requested estimate:

$$
\boxed{\left|\int_{\mathbb R^2}f(x,y)\,dx\,dy\right|
\leq\int_{\mathbb R^2}|f(x,y)|\,dx\,dy
\leq8\int_{\mathbb R}|g(y)|\,dy.}
$$

This is the [L1 norm identity for a translated kernel product](../../../../l1-norm-identity-for-a-translated-kernel-product.md) followed by a simple bound on the [convolution kernel](../../../../convolution-kernel.md).

There is also a stronger signed conclusion. The integrable [convolution kernel](../../../../convolution-kernel.md) $k$ is an [odd function](../../../../odd-function.md), so $\int_{\mathbb R}k(t)\,dt=0$. Having established [absolute integrability](../../../../integrability.md), we may apply [Fubini's theorem](../../../../fubini-s-theorem.md) to $f$ itself:

$$
\boxed{\int_{\mathbb R^2}f(x,y)\,dx\,dy
=\left(\int_{\mathbb R}k(t)\,dt\right)\left(\int_{\mathbb R}g(y)\,dy\right)=0.}
$$

Unlike part (a), the signed cancellation is justified by a finite [integral](../../../../integral-split.md) of the [absolute value](../../../../absolute-value.md). The constant eight is useful as an [L1 norm](../../../../l1-norm.md) bound even though this particular signed total vanishes.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
