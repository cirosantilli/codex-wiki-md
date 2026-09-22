<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Work on the common [probability space](../../../../../../probability-space.md) from part (c). For a configuration of all the uniforms, the [set](../../../../../../set-split.md) $S=\{r\in[0,1]:I_r\text{ occurs}\}$ is an upper interval, possibly with or without its lower endpoint. It is nonempty because $I_1$ occurs, and the [coupled onset parameter for origin percolation](../../../../../../coupled-onset-parameter-for-origin-percolation.md) is $M=\inf S$. For $0<p\leq1$,

$$
\bigcup_{\substack{r<p\\r\in\mathbb Q\cap[0,1]}} I_r=\{M<p\}.
$$

Indeed, occurrence at some $r<p$ implies $M<p$. Conversely, if $M<p$, the definition of infimum yields occurrence at some $s<p$, and a rational $r$ between $s$ and $p$ also satisfies $I_r$. This also proves measurability of $M$ through its strict sublevel [sets](../../../../../../set-split.md).

Choose a rational sequence increasing to $p$. By [continuity from below of a measure](../../../../../../continuity-from-below-of-a-measure.md) and the [monotone coupling of Bernoulli percolation](../../../../../../monotone-coupling-of-bernoulli-percolation.md),

$$
\lim_{r\uparrow p}\theta(r)=\mathbb P(M<p).
$$

Moreover, $\{M<p\}\subseteq I_p\subseteq\{M\leq p\}$. Hence $I_p$ is the disjoint union of $\{M<p\}$ and $I_p\cap\{M=p\}$, giving

$$
\boxed{\lim_{r\uparrow p}\theta(r)=\theta(p)-\mathbb P(I_p\cap\{M=p\})}.
$$

It is important to retain the intersection with $I_p$: occurrence at the infimum is not automatic. At $p=0$ there is no left limit within the parameter domain, so the displayed left-limit assertion is for $p>0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
