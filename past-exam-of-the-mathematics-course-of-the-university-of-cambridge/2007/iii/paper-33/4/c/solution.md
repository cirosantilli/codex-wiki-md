<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Borel-Cantelli first lemma](../../../../../../borel-cantelli-first-lemma.md) applied to that finite sum says that almost surely, for all sufficiently large $n$,

$$
S_{2^{-n-1}}\geq2^{-n/2}f(2^{-n}).
$$

For $2^{-n-1}\leq t\leq2^{-n}$, both the [Brownian running maximum](../../../../../../brownian-running-maximum.md) and the positive function $\sqrt t\,f(t)$ are nondecreasing. Thus eventually

$$
S_t\geq S_{2^{-n-1}}\geq\sqrt{2^{-n}}\,f(2^{-n})\geq\sqrt t\,f(t).
$$

This proves the lower limit bound one, with interpolation across all small real times rather than only the dyadic sequence.

For every positive integer $m$, the function $mf$ satisfies the same assumptions and integrability condition. Repeating the argument gives an eventual lower bound $S_t\geq m\sqrt t f(t)$ on a probability-one event. Take the countable intersection of these events. On it, the ratio is eventually at least any prescribed positive integer, proving the [integral lower envelope for the Brownian maximum](../../../../../../integral-lower-envelope-for-the-brownian-maximum.md):

$$
\boxed{\liminf_{t\downarrow0}\frac{S_t}{\sqrt t\,f(t)}=\infty\quad\text{almost surely}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
