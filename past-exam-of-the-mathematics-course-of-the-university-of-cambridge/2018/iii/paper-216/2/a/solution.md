<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the planar [uniform distribution](../../../../../../continuous-uniform-distribution.md) with a [Lebesgue measure](../../../../../../lebesgue-measure.md) density, assume that the compact [convex set](../../../../../../convex-set.md) $\mathcal C$ has nonempty interior, equivalently positive area. This assumption is missing from the wording: a line segment or singleton would not have such a planar uniform density.

The [hit-and-run sampler](../../../../../../hit-and-run-sampler.md) at a current point $x$ chooses $u=(\cos\Theta,\sin\Theta)$ with $\Theta$ uniform on $[0,2\pi)$, finds the interval

$$
I(x,u)=\{t:x+tu\in\mathcal C\}=[t_-(x,u),t_+(x,u)],
$$

and samples $T$ uniformly on that interval, setting $x'=x+Tu$. Convexity makes the intersection an interval and compactness makes it bounded.

If $x$ is in the interior, every direction has positive chord length, and the next point is in the interior almost surely. For a definition valid at every boundary point as well, redraw the direction whenever the chord has zero length. We use this convention in the following parts. Positive-length directions have positive angular probability at every $x$, since an interior ball is visible from $x$, so the redraw terminates almost surely.

The [Markov kernel](../../../../../../markov-kernel.md) has the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $\mathcal C$ as its invariant law, as follows from the density symmetry proved next. Repeating the step therefore produces approximate uniform samples after convergence. The boundary convention matters: if singleton chords were instead treated as holding moves, a square's corner would have a positive atom at its starting point, contradicting part (b)'s claim of an everywhere absolutely continuous kernel.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
