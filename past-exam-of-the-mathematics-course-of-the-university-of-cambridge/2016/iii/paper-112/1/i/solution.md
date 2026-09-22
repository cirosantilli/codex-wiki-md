<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\lambda_n$ for [Lebesgue measure](../../../../../../lebesgue-measure.md) on $\mathbb R^n$. The [Prékopa–Leindler inequality](../../../../../../prekopa-leindler-inequality.md) says that if $0<\theta<1$ and nonnegative [measurable functions](../../../../../../measurable-function.md) $f,g,h$ satisfy

$$
h((1-\theta)x+\theta y)\geq f(x)^{1-\theta}g(y)^\theta\qquad(x,y\in\mathbb R^n),
$$

then their [Lebesgue integrals](../../../../../../lebesgue-integral.md) satisfy

$$
\boxed{\int h\geq\left(\int f\right)^{1-\theta}\left(\int g\right)^\theta.}
$$

It suffices initially to take $0<\int f,\int g<\infty$. Zero integrals give a trivial bound; infinite integrals can be handled by truncating $f$ and $g$ and applying the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md). As usual, a zero factor makes the asserted lower bound zero.

Here is a one-dimensional proof using [quantile functions](../../../../../../quantile-function.md). Put $F=\int f$, $G=\int g$, and let $x(u),y(u)$, $0<u<1$, be the [quantile functions](../../../../../../quantile-function.md) of the [probability density functions](../../../../../../probability-density-function.md) $f/F$ and $g/G$. At almost every $u$ the [quantile derivative identity](../../../../../../quantile-derivative-identity.md) gives

$$
a(u):=x'(u)=\frac{F}{f(x(u))}>0,\qquad b(u):=y'(u)=\frac{G}{g(y(u))}>0.
$$

For completeness, these reciprocal derivative identities follow by differentiating the corresponding [cumulative distribution functions](../../../../../../cumulative-distribution-function.md) at their [Lebesgue points](../../../../../../lebesgue-point.md) and then differentiating the [inverse function](../../../../../../inverse-function.md) relation. Sampling a [quantile function](../../../../../../quantile-function.md) at a uniform argument samples the density itself, so the exceptional set, including locations where the density vanishes or is infinite, has probability zero. Gaps in a density's support can give jumps in its [quantile function](../../../../../../quantile-function.md); they do not invalidate the argument below.

The [monotone function](../../../../../../monotonic-function.md) $z(u)=(1-\theta)x(u)+\theta y(u)$ obeys the [monotone substitution inequality](../../../../../../monotone-substitution-inequality.md):

$$
\int_{\mathbb R}h(s)\,ds\geq\int_0^1 h(z(u))z'(u)\,du.
$$

This form uses the ordinary [derivative](../../../../../../derivative.md) of a [monotone function](../../../../../../monotonic-function.md), rather than any jump or singular part: its weighted image measure is dominated by [Lebesgue measure](../../../../../../lebesgue-measure.md). One can see this first for intervals, where $\int_{z^{-1}(I)}z'\leq\lambda_1(I)$, and then extend to nonnegative [measurable functions](../../../../../../measurable-function.md) by [simple function](../../../../../../simple-function.md) approximation. Thus no assumption of strictly positive smooth [probability density functions](../../../../../../probability-density-function.md) is hidden in the proof.

Using the hypothesis and the weighted [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md), we obtain

$$
\begin{aligned}
h(z(u))z'(u)&\geq F^{1-\theta}G^\theta\frac{(1-\theta)a(u)+\theta b(u)}{a(u)^{1-\theta}b(u)^\theta}\\
&\geq F^{1-\theta}G^\theta.
\end{aligned}
$$

Integrating over $0<u<1$ proves the one-dimensional [Prékopa–Leindler inequality](../../../../../../prekopa-leindler-inequality.md).

For higher dimensions, use [mathematical induction](../../../../../../mathematical-induction.md) and [Tonelli theorem](../../../../../../tonelli-theorem.md). Write $x=(x',s)$ and set

$$
F_1(x')=\int_{\mathbb R}f(x',s)\,ds,\qquad G_1(y')=\int_{\mathbb R}g(y',t)\,dt,\qquad H_1(z')=\int_{\mathbb R}h(z',r)\,dr.
$$

Apply the one-dimensional [Prékopa–Leindler inequality](../../../../../../prekopa-leindler-inequality.md) to the last-coordinate slices, with $z'=(1-\theta)x'+\theta y'$. It gives

$$
H_1((1-\theta)x'+\theta y')\geq F_1(x')^{1-\theta}G_1(y')^\theta.
$$

Apply the induction hypothesis in $\mathbb R^{n-1}$ and use [Tonelli theorem](../../../../../../tonelli-theorem.md) once more. For finite total integrals, infinite slice integrals occur only on null sets and may be replaced by zero there; this only weakens the displayed premise. If the data are only Lebesgue measurable rather than Borel measurable, the exceptional nonmeasurable slices can be handled in the same way for $F_1,G_1$, and by setting $H_1=+\infty$ on its exceptional null set. The total integrals are unchanged, and the slice premise holds everywhere it is needed. **The result therefore holds for general nonnegative measurable functions.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
