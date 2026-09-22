# Remainder of a geometric series

↑ **Parent:** [Geometric series](geometric-series.md)

For $|r|<1$, let $S_N$ contain the first $N$ terms, with $S_0=0$. The remainder after those terms is

$$
R_N=\sum_{j=N}^{\infty}ar^j=\frac{ar^N}{1-r},
\qquad
\left|\frac{a}{1-r}-S_N\right|
=\frac{|a|\,|r|^N}{|1-r|}.
$$

This is the exact [absolute error](absolute-error.md). A convenient bound replaces the denominator by $1-|r|$, giving $|R_N|\le |a|\,|r|^N/(1-|r|)$ through the [triangle inequality](triangle-inequality.md). The exact denominator is preferable when the sign or complex phase of $r$ is known.

<a id="image-the-omitted-fraction-and-the-number-of-terms-needed-to-capture-99-percent-of-a-geometric-sum"></a>
![](geometric-series-remainder-and-term-count.png)

**[Figure 32](#image-the-omitted-fraction-and-the-number-of-terms-needed-to-capture-99-percent-of-a-geometric-sum). The omitted fraction and the number of terms needed to capture 99 percent of a geometric sum**.

For $a>0$ and $0<r<1$, the omitted fraction of the entire sum is $R_N/(a/(1-r))=r^N$. Capturing at least $99$ percent therefore means $r^N\le0.01$. Taking [logarithms](logarithm.md) and applying the [ceiling function](ceiling-function.md) gives the smallest [integer](integer.md) $N$:

$$
N=\left\lceil\frac{\log(0.01)}{\log r}\right\rceil.
$$

This gives $7,21,90,$ and $459$ terms for $r=0.5,0.8,0.95,$ and $0.99$, respectively. The difference is a concrete reason to care about the [common ratio](common-ratio.md), even when all four series converge.

An absolute target has a different scale. For $a=1$, $r=0.8$, and required [absolute error](absolute-error.md) at most $0.01$, the total sum is $5$ and

$$
|R_N|=5(0.8)^N\le0.01.
$$

The first acceptable term count is $N=28$: the remainder is approximately $0.0096714$, while at $N=27$ it is approximately $0.0120893$. Counting terms and checking the tail avoids an ambiguous instruction to stop when a term merely looks small.

## ↑ Ancestors (7)

1. [Geometric series](geometric-series.md)
2. [Sequence and series](sequence-and-series.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Geometric series](geometric-series.md)
