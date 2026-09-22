# Increasing-subsequence certificate concentration

↑ **Parent:** [Talagrand concentration inequality for certifiable functions](talagrand-concentration-inequality-for-certifiable-functions.md)

For the [longest increasing subsequence](longest-increasing-subsequence.md) length $L$ on a product space of independent coordinates, a witness of length $\ell$ uses only $\ell$ coordinates. Any point with subsequence length at most $a$ must differ on at least $\ell-a$ witness positions. Weights $1/\sqrt\ell$ on those positions show $d_T(x,\{L\leq a\})\geq(\ell-a)/\sqrt\ell$. Thus for $0\leq a<b$,

$$
\Pr(L\leq a)\Pr(L\geq b)\leq e^{-(b-a)^2/(4b)}.
$$

At a [median](median.md) $m$, this gives upper tail $2e^{-t^2/[4(m+t)]}$ and lower tail $2e^{-t^2/(4m)}$. Integrating the tails places the mean within $O(\sqrt m+1)$ of the [median](median.md), so the natural concentration scale near the mean is $\sqrt{\mathbb EL}$. A random permutation is represented by the ranks of independent continuous variables; arbitrary dependent sequences need not obey this conclusion.

## ↑ Ancestors (9)

1. [Talagrand concentration inequality for certifiable functions](talagrand-concentration-inequality-for-certifiable-functions.md)
2. [Talagrand's concentration inequality](talagrand-s-concentration-inequality.md)
3. [Concentration inequality](concentration-inequality.md)
4. [Probability inequality](probability-inequality-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/5/solution.md)
