<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $0<\delta<1$, define the compensated small-jump [Poisson integral](../../../../../../poisson-integral.md)

$$
Y_t^\delta=\int_{(0,t]\times\{\delta<|y|\leq1\}}y\,(\mu-\nu)(dy,ds).
$$

This is an ordinary compensated finite-intensity sum. [Independent](../../../../../../independent-random-variables.md) [Poisson random variables](../../../../../../poisson-distribution.md) give mean zero and the [L2 construction of compensated Poisson integrals](../../../../../../l2-construction-of-compensated-poisson-integrals.md) gives, for $0<\eta<\delta$,

$$
\mathbb E|Y_t^\eta-Y_t^\delta|^2=t\int_{\{\eta<|y|\leq\delta\}}y^2K(dy)=2ct(\delta-\eta).
$$

Thus $Y_t^\delta$ is [Cauchy](../../../../../../cauchy-sequence.md) in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) as $\delta\downarrow0$, defining the first integral. It is not the difference of two separately convergent integrals. On a compact time interval $[0,L]$, the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) bounds the squared supremum of the same difference by $8cL(\delta-\eta)$. Hence the truncated [martingales](../../../../../../martingale-split.md) are Cauchy in the expected squared supremum norm. A sufficiently rapidly decreasing sequence of cutoffs converges uniformly [almost surely](../../../../../../almost-sure-convergence.md); its limit has [càdlàg](../../../../../../cadlag.md) paths, so the construction also supplies a consistent process.

For large jumps, $K(\{|y|>1\})=2c<\infty$. There are only finitely many such atoms before any fixed time, [almost surely](../../../../../../almost-sure-convergence.md), and each atom has a finite mark. The uncompensated large-jump integral is therefore a finite random sum, even though its absolute first moment is infinite. The two terms are well-defined for these different reasons.

There is also a literal signed-integral defect in the PDF: $\int yK(dy)$ on either symmetric region is not $+\infty$. Its positive and negative parts both have infinite mass, so the ordinary signed [Lebesgue integral](../../../../../../lebesgue-integral.md) is undefined. The correct divergence statement is

$$
\int_{0<|y|\leq1}|y|K(dy)=\int_{|y|>1}|y|K(dy)=\infty.
$$

A symmetric principal value may be zero, but is not an ordinary signed integral. **Square-integrable compensation defines the small jumps; finite activity defines the large jumps.**

## ↑ Ancestors (11)

1. [A](../a.md)
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
