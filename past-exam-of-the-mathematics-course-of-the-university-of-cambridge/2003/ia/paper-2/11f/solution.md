<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

An uneventful day leaves one aphid, a one-offspring day leaves the parent plus its offspring, and a two-offspring day leaves three aphids. Death leaves none. Thus the daily descendant counts are $0,1,2,3$ with [probabilities](../../../../../probability.md) $(1-q)t$, $q$, $(1-q)r$, $(1-q)s$, respectively. The [mean](../../../../../expected-value.md) and [probability generating function](../../../../../probability-generating-function.md) are

$$
\boxed{\mathbb EX_1=q+(1-q)(2r+3s),\qquad
G(z)=(1-q)t+qz+(1-q)rz^2+(1-q)sz^3.}
$$

Independence across individuals and days makes the daily population a [Galton-Watson process](../../../../../galton-watson-process.md), with each surviving parent counted as one of the next day's descendants.

The standard [Galton-Watson extinction fixed point](../../../../../galton-watson-extinction-fixed-point.md) result states that the eventual [extinction probability of a branching process](../../../../../extinction-probability-of-a-branching-process.md) $e$ from one ancestor is the smallest root in $[0,1]$ of $G(e)=e$. Moreover a nondegenerate offspring law of [mean](../../../../../expected-value.md) at most one has [extinction probability of a branching process](../../../../../extinction-probability-of-a-branching-process.md) one. Here, since $q<1$, the fixed-point equation reduces to

$$
\boxed{e=t+re^2+se^3,}
$$

which contains no $q$. This proves [laziness invariance of branching extinction](../../../../../laziness-invariance-of-branching-extinction.md): uneventful days change the timescale, not eventual extinction. The excluded case $q=1$ would keep one aphid forever.

If $2r+3s\le1$, the offspring [mean](../../../../../expected-value.md) is at most one. In this parameter range $t>0$: if $t=0$, then $r+s=1$ would imply $2r+3s\ge2$. Thus the offspring law is not deterministically one, and the extinction criterion applies. **Extinction is certain.**

For the specified [probabilities](../../../../../probability.md), the fixed-point equation factors as

$$
2e^3+e^2-5e+2=(e-1)(2e-1)(e+2)=0.
$$

Its roots in $[0,1]$ are $1/2$ and $1$, and the smaller root is the [extinction probability of a branching process](../../../../../extinction-probability-of-a-branching-process.md):

$$
\boxed{e=\frac12.}
$$

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
