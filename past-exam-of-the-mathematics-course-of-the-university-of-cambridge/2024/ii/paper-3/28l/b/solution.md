<h1 id="28l/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The $\pi$-Bayes risk is

$$
r_\pi(\delta)=\int R(\delta,\theta)\,\pi(d\theta).
$$

Conditioning on the observation and applying Tonelli gives

$$
r_\pi(\delta)=\mathbb E_{X}\left[
\mathbb E\{L(\delta(X),\theta)\mid X\}
\right].
$$

**Thus choosing, for every observed $x$, an action minimizing the posterior expected loss minimizes each integrand and hence minimizes the Bayes risk.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28L](../../28l.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
