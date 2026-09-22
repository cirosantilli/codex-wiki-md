# Big theta notation

↑ **Parent:** [Big O notation](big-o-notation.md)

At the specified [limit](limit-of-a-function.md), big theta notation means that two positive constants give both-sided bounds:

$$
\boxed{c|g|\le |f|\le C|g|\qquad(0<c\le C)}
$$

sufficiently near the [limit](limit-of-a-function.md). Equivalently, $f=O(g)$ and $g=O(f)$ in [big O notation](big-o-notation.md). In operation-count analysis, $3n^2+7n+4=\Theta(n^2)$ for $n\ge1$, using $c=3$ and $C=14$. This supplies a tight scale without asserting that the normalized ratio tends to one.

For an example with no limiting ratio, let $f(n)=n(2+(-1)^n)$ for positive [integers](integer-split.md) $n$. Then $n\le f(n)\le3n$, so $f(n)=\Theta(n)$, but $f(n)/n$ alternates between one and three. A tight growth order is therefore weaker than [asymptotic equivalence](asymptotic-equivalence.md). The constant bounds also do not fix an exact factor by which a function changes when its argument doubles.

Donald E. Knuth's 1976 paper proposes using $\Theta$ for two-sided constant bounds in algorithm analysis. He credits Bob Tarjan and Mike Paterson with independently suggesting the notation. His discussion gives a concrete motivation for distinguishing an eventual upper estimate from a tight comparison. [Knuth, Big Omicron and big Omega and big Theta, 1976, pages 19–20](https://danluu.com/knuth-big-o.pdf)

## ↑ Ancestors (6)

1. [Big O notation](big-o-notation.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Asymptotic analysis](asymptotic-analysis.md)
- [Asymptotic equivalence](asymptotic-equivalence.md)
- [Big O notation](big-o-notation.md)
