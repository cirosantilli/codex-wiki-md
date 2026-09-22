<h1 id="11f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The geometric family law on the nonnegative integers has [probability generating function](../../../../../../probability-generating-function.md)

$$
\boxed{G(s)=\sum_{k\geq0}2^{-k-1}s^k=\frac1{2-s}},\qquad |s|<2.
$$

Its [expected value](../../../../../../expected-value.md) is $G'(1)=1$, so this is a [geometric-offspring critical branching process](../../../../../../geometric-offspring-critical-branching-process.md). Starting from $G_0(s)=s$, verify the rational iterate by induction. If $G_n(s)=[n-(n-1)s]/[n+1-ns]$, then

$$
G(G_n(s))=\frac1{2-G_n(s)}=\frac{n+1-ns}{n+2-(n+1)s},
$$

which has the same form with $n$ replaced by $n+1$. Thus, for $n\geq1$,

$$
\boxed{G_n(s)=\frac{n-(n-1)s}{n+1-ns},\qquad |s|<1+\frac1n}.
$$

The stated disk is the actual power-series convergence domain, not merely a place where the rational continuation can be evaluated. Its simple pole is at $s=1+1/n$.

The extinction [probability](../../../../../../probability.md) at generation $n$ is the constant coefficient:

$$
\boxed{P(X_n=0)=G_n(0)=\frac n{n+1}}.
$$

For later use, expanding the remaining [geometric series](../../../../../../geometric-series.md) gives

$$
P(X_n=j)=\frac1{(n+1)^2}\left(\frac n{n+1}\right)^{j-1},\qquad j\geq1.
$$

In particular $P(X_n>0)=1/(n+1)$. At $n=0$ the initial population is one deterministically; its [PGF](../../../../../../probability-generating-function.md) is $s$, and the displayed radius involving $1/n$ is used only for $n\geq1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
