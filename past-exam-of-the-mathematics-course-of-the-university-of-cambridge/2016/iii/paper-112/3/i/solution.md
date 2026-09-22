<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The useful form is [Talagrand's convex distance inequality](../../../../../../talagrand-s-convex-distance-inequality.md). Let $(\Omega_i,\mu_i)$ be standard [probability spaces](../../../../../../probability-space.md), let $\Omega=\prod_{i=1}^n\Omega_i$ carry the [product measure](../../../../../../product-measure.md) $\mu=\bigotimes_i\mu_i$, and let $A\subset\Omega$ be a measurable event with $\mu(A)>0$. For $x\in\Omega$, form the mismatch vectors

$$
V_A(x)=\{(\mathbf1_{x_i\ne y_i})_{i=1}^n:y\in A\}.
$$

The [Talagrand convex distance](../../../../../../talagrand-convex-distance.md) is the distance from zero to their closed [convex hull](../../../../../../convex-hull.md):

$$
d_T(x,A)=\inf\{\lVert v\rVert_2:v\in\overline{\operatorname{conv}}V_A(x)\}.
$$

Equivalently, by the [Hahn-Banach separation theorem for two convex sets](../../../../../../hahn-banach-separation-theorem-for-two-convex-sets.md),

$$
d_T(x,A)=\sup_{\substack{\alpha_i\geq0\\\sum_i\alpha_i^2\leq1}}\ \inf_{y\in A}\sum_{i:x_i\ne y_i}\alpha_i.
$$

Nonnegative weights suffice because every mismatch vector has nonnegative coordinates. [Talagrand's convex distance inequality](../../../../../../talagrand-s-convex-distance-inequality.md) states

$$
\boxed{\int_\Omega\exp(d_T(x,A)^2/4)\,d\mu(x)\leq\frac1{\mu(A)}.}
$$

In particular, [Markov's inequality](../../../../../../markov-inequality.md) gives the product-space [concentration inequality](../../../../../../concentration-inequality.md)

$$
\boxed{\mu(A)\,\mu\{x:d_T(x,A)\geq s\}\leq e^{-s^2/4}\qquad(s>0).}
$$

The same conclusion is interpreted with outer probabilities if a distance set is not measurable; the continuous geometric function used below has measurable level sets. A [median](../../../../../../median.md) $M$ of a real [random variable](../../../../../../random-variable-split.md) $Z$ means that $\mathbb P(Z\leq M)\geq1/2$ and $\mathbb P(Z\geq M)\geq1/2$. Applying the displayed [concentration inequality](../../../../../../concentration-inequality.md) to suitable level sets will control deviations around a [median](../../../../../../median.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
