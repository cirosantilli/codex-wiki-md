<h1 id="20c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Until the first visit to zero, the positive-side chain is a nearest-neighbour random walk with upward probability $2/3$ and downward probability $1/3$. For an [integer](../../../../../../integer.md) $m>1$, let $h_i^{(m)}=\Pr_i(T_0<T_m)$, $0\leq i\leq m$. The [Markov property](../../../../../../markov-property.md) gives

$$
h_i^{(m)}=\frac13h_{i-1}^{(m)}+\frac23h_{i+1}^{(m)},\qquad h_0^{(m)}=1,\quad h_m^{(m)}=0.
$$

The characteristic roots of this recurrence are $1$ and $1/2$. Solving its two boundary equations gives the [biased gambler's ruin probability](../../../../../../biased-gambler-s-ruin-probability.md)

$$
h_i^{(m)}=\frac{2^{-i}-2^{-m}}{1-2^{-m}}.
$$

A finite path that reaches zero has a finite maximum before doing so, and is counted by $\{T_0<T_m\}$ for every sufficiently large $m$. Conversely each such event implies a visit to zero. Therefore these events increase to $\{T_0<\infty\}$, and [continuity](../../../../../../continuous-function.md) of probability gives

$$
\boxed{\Pr_1(T_0<\infty)=\lim_{m\to\infty}h_1^{(m)}=\frac12.}
$$

More generally the hitting probability from $i>0$ is $2^{-i}$. The finite-boundary derivation avoids choosing an unjustified solution of the infinite recurrence.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20C](../../20c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
