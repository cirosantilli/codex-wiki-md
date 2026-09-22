# Asymptotic comparison of exponential functions

↑ **Parent:** [Asymptotic equivalence](asymptotic-equivalence.md)

For positive bases $a,b$, comparison of the [exponential functions](exponential-function.md) $a^n$ and $b^n$ reduces to a [geometric progression](geometric-progression.md):

$$
\frac{a^n}{b^n}=\left(\frac ab\right)^n.
$$

If $a<b$, this ratio tends to zero, so $a^n=o(b^n)$ in [little o notation](little-o-notation.md). If $a=b$, the ratio is one; if $a>b$, it grows without bound.

Consequently, provided at least one coefficient is nonzero, a finite sum with distinct positive bases is [asymptotically equivalent](asymptotic-equivalence.md) to its largest-base term whose coefficient is nonzero. For example,

$$
3\cdot2^n+5\cdot3^n\sim5\cdot3^n,\qquad
\frac{3\cdot2^n+5\cdot3^n}{5\cdot3^n}
=1+\frac35\left(\frac23\right)^n.
$$

The relative difference against $5\cdot3^n$ first drops below one percent at the integer $n=11$. Dividing by the proposed dominant term provides an explicit error estimate, not just a comparison of two rapidly growing numbers. If several terms have the same largest base, their coefficients must first be combined; cancellation can remove that base entirely.

## ↑ Ancestors (7)

1. [Asymptotic equivalence](asymptotic-equivalence.md)
2. [Asymptotic analysis](asymptotic-analysis.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Asymptotic analysis](asymptotic-analysis.md)
- [Big O notation](big-o-notation.md)
