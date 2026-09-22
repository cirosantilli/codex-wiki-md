<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Disjoint time strips of the [Poisson random measure](../../../../../../poisson-random-measure.md) are [independent](../../../../../../independent-random-variables.md), and its intensity is translation invariant in time. The construction and its limits therefore give [independent increments](../../../../../../independent-increments.md) and [stationary increments](../../../../../../stationary-increments.md), with

$$
\mathbb E e^{iu(X_t-X_s)}=e^{-(t-s)|u|}\qquad(0\leq s<t).
$$

For the scaling actually printed in the original PDF,

$$
\mathbb E e^{iu\alpha X_{\alpha t}}=e^{-\alpha^2t|u|}.
$$

For example, $\alpha=2$, $t=1$, $u=1$ gives $e^{-4}$ rather than $e^{-1}$. Thus **the requested equality of process laws is false unless $\alpha=1$**.

The intended [self-similarity of a Cauchy process](../../../../../../self-similarity-of-a-cauchy-process.md) rescales space and time in opposite directions:

$$
\boxed{\left(\alpha^{-1}X_{\alpha t}\right)_{t\geq0}\stackrel{d}=(X_t)_{t\geq0}}
\qquad\text{or equivalently}\qquad
\boxed{\left(\alpha X_{t/\alpha}\right)_{t\geq0}\stackrel{d}=(X_t)_{t\geq0}}.
$$

Indeed, for $0\leq s<t$,

$$
\mathbb E\exp\left[iu\alpha^{-1}(X_{\alpha t}-X_{\alpha s})\right]
=\exp\left[-\alpha(t-s)|u|/\alpha\right]=e^{-(t-s)|u|}.
$$

The transformed process retains [independent increments](../../../../../../independent-increments.md). For any ordered times, the joint [characteristic function](../../../../../../characteristic-function.md) of its successive increments is therefore the same product as for $X$; cumulative summation proves equality of all [finite-dimensional distributions](../../../../../../finite-dimensional-distribution.md). Both constructions have [càdlàg](../../../../../../cadlag.md) paths, so these distributions also determine their laws on the usual [path space](../../../../../../path-space.md). This derives the corrected invariance and explicitly diagnoses the false printed assertion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
