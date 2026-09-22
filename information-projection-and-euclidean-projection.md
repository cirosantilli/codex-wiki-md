# Information projection and Euclidean projection

↑ **Parent:** [Information projection on three outcomes](information-projection-on-three-outcomes.md)

The word "projection" does not mean ordinary perpendicular projection in the plotted [Euclidean space](euclidean-norm.md). For the same reference and [mean](expected-value-split.md) constraint, minimizing the squared [Euclidean distance](euclidean-distance.md) in the three [probability](probability.md) coordinates instead gives

$$
\sum_i(q_i-1/3)^2=6x^2-x+\frac16,
\qquad x_{\mathrm E}=\frac1{12}.
$$

Thus the Euclidean minimizer is $q_{\mathrm E}=(1/12,1/3,7/12)$, whereas the [information projection](information-projection.md) has $q_-^*\approx0.116204$. The squared Euclidean objective at its own minimum is $1/8$; its [relative entropy](kullback-leibler-divergence.md) is approximately $0.210918$ [nats](nat-unit.md), larger than the optimum $0.197378$ [nats](nat-unit.md). Both distributions satisfy the same constraint.

<a id="image-relative-entropy-and-least-squares-select-different-laws-under-the-same-mean-constraint"></a>
![](information-projection-relative-entropy-versus-least-squares.png)

**[Figure 16](#image-relative-entropy-and-least-squares-select-different-laws-under-the-same-mean-constraint). Relative entropy and least squares select different laws under the same mean constraint**. Both plots use the feasible laws $q=(x,1/2-2x,1/2+x)$ and the same uniform reference. The left plot minimizes [relative entropy](kullback-leibler-divergence.md); the right plot minimizes squared [Euclidean distance](euclidean-distance.md) in the three probability coordinates. Their different marked minima explain why the choice of objective matters.

The reference and objective encode what "least change" means. [Relative entropy](kullback-leibler-divergence.md) is asymmetric and is not a [metric](metric.md); its minimization answers a different question from [linear least squares](linear-least-squares.md). The useful geometric analogy comes from a [Pythagorean inequality for information projection](pythagorean-inequality-for-information-projection.md), rather than from an assertion that the colored contours are circles.

## ↑ Ancestors (9)

1. [Information projection on three outcomes](information-projection-on-three-outcomes.md)
2. [Information projection](information-projection.md)
3. [Method of types](method-of-types.md)
4. [Type (information theory)](type-information-theory.md)
5. [Information theory](information-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
