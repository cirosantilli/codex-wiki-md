<h1 id="2/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**This [covariance](../../../../../../../covariance.md) is also zero, but symmetry is essential to the proof.** Write $\varepsilon_t=\eta_t|\varepsilon_t|$, where $\eta_t$ is an independent fair sign. The [normal distribution](../../../../../../../normal-distribution.md) makes that sign independent of its magnitude and of every other driving variable. Conditional on the magnitudes and all noise except this sign, changing $\eta_t$ flips $X_t$ and leaves $X_t^2$ unchanged. Every future conditional scale uses only squared past observations, so $X_{t+h}$ is unchanged for $h>0$.

Thus $f(X_{t+h})$ is independent of the remaining fair sign in $X_t$. Averaging that sign gives $\mathbb E[X_tf(X_{t+h})]=0$, and hence

$$
\boxed{\operatorname{Cov}(X_t,f(X_{t+h}))=0.}
$$

The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) again guarantees integrability. For odd $h$, the [parity decomposition of a lag-two ARCH process](../../../../../../../parity-decomposition-of-a-lag-two-arch-process.md) also gives [independence](../../../../../../../independent-random-variables.md) directly. For even $h$, the [sign symmetry of an ARCH process](../../../../../../../sign-symmetry-of-an-arch-process.md) supplies the argument; the [martingale difference sequence](../../../../../../../martingale-difference-sequence.md) property alone would not justify this reversed [covariance](../../../../../../../covariance.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [2](../../../2.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
