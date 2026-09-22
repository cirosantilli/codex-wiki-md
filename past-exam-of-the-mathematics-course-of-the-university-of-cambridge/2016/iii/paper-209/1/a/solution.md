<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\delta_i=t_i-t_{i-1}$, $\Delta=\max_i\delta_i$, $v_i=\int_{t_{i-1}}^{t_i}\sigma(s)^2\,ds$ and $S=\|\sigma^4\|_\infty$. The deterministic integrand in the [Itô integral](../../../../../../ito-integral.md) implies that the increments $Z_i=X_{t_i}-X_{t_{i-1}}$ are [independent random variables](../../../../../../independent-random-variables.md) with [normal distributions](../../../../../../normal-distribution.md) $N(0,v_i)$. The [Gaussian fourth moment](../../../../../../gaussian-fourth-moment.md) gives

$$
\mathbb E Z_i^2=v_i,\qquad \mathbb E Z_i^4=3v_i^2,\qquad \operatorname{Var}(Z_i^2)=2v_i^2.
$$

These identities include $v_i=0$. Since the summands of $M_n$ are centered and [independent](../../../../../../independent-random-variables.md), all cross terms in its [second moment](../../../../../../second-moment.md) vanish. Consequently,

$$
\mathbb E M_n^2=2\sum_{i=1}^n g(t_{i-1})^2v_i^2
\leq2R^2S\sum_{i=1}^n\delta_i^2
\leq2R^2S\Delta\sum_{i=1}^n\delta_i
=2R^2S\Delta.
$$

Thus **$D=2$ works for every observation partition**. The last step uses the total interval length, rather than assuming equally spaced observations.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
