<h1 id="4/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Kolmogorov continuity theorem](../../../../../../kolmogorov-continuity-theorem.md) in its one-parameter form: if on a compact interval a process satisfies $\mathbb E|X_t-X_s|^p\leq C|t-s|^{1+\beta}$ for some $p,\beta>0$, it has a modification whose paths are [Hölder continuous](../../../../../../holder-condition.md) of every order $\gamma<\beta/p$ on that interval.

For [Brownian motion](../../../../../../brownian-motion-split.md), normal increments give, for every $p>0$,

$$
\mathbb E|B_t-B_s|^p=\mathbb E|Z|^p\,|t-s|^{p/2},\qquad Z\sim N(0,1).
$$

Every such normal moment is finite. Taking $p>2$ yields $\beta=p/2-1$, hence any order below $1/2-1/p$. For a prescribed $0<\alpha<1/2$, choose $p$ with $1/2-1/p>\alpha$.

The continuous modification and the given continuous [Brownian motion](../../../../../../brownian-motion-split.md) agree at all rational times on one [almost sure event](../../../../../../almost-sure-event.md); continuity makes them agree everywhere on the interval. To obtain all exponents and all compact intervals simultaneously, apply the theorem to integer intervals $[0,N]$ and a countable sequence of positive exponents increasing to $1/2$, then intersect these [almost sure events](../../../../../../almost-sure-event.md). A bound at exponent $\gamma>\alpha$ implies a bound at $\alpha$ on a compact interval. Consequently the [Brownian Hölder regularity](../../../../../../brownian-holder-regularity.md) conclusion is

$$
\boxed{|B_t-B_s|\leq C_{N,\alpha}|t-s|^\alpha\quad(s,t\in[0,N]),\qquad0<\alpha<\tfrac12,}
$$

with finite random constants on one common event of probability one. This uses the usual positive-exponent meaning of Hölder continuity.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [4](../../4.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
