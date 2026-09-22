<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md), the increments have mean $0$ and [variance](../../../../../../variance-split.md) $1$. Use the polygonal interpolation from (b). The maximum functional is Lipschitz in the [supremum norm](../../../../../../supremum-norm.md), since

$$
\left|\max_{0\leq s\leq1}g(s)-\max_{0\leq s\leq1}h(s)\right|\leq\|g-h\|_\infty.
$$

Each interpolating segment is linear, so its maximum occurs at a grid endpoint. The [continuous mapping theorem](../../../../../../continuous-mapping-theorem.md) applied to the [Donsker invariance principle](../../../../../../donsker-s-theorem.md) gives

$$
\frac1{\sqrt n}\max_{0\leq j\leq n}S_j\ \Rightarrow\ \max_{0\leq s\leq1}B_s.
$$

The limiting maximum has no atom at $a>0$ by the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md), so the closed-tail [probabilities](../../../../../../probability.md) converge at this threshold. Including $j=0$ does not change the event because $a>0$. Therefore the [random-walk maximum limit from Donsker invariance](../../../../../../random-walk-maximum-limit-from-donsker-invariance.md) is

$$
\boxed{\lim_{n\to\infty}\mathbb P\left(\max_{j\leq n}S_j\geq a\sqrt n\right)=2\bigl(1-\Phi(a)\bigr),\qquad a>0.}
$$

Here $\Phi$ is the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md). The normalization and the positive-threshold condition are those in the PDF; the TeX aid's $\sqrt t$ is not the printed expression.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
