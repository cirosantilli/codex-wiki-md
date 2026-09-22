# Bounded monotone sequences have no universal convergence rate

↑ **Parent:** [Error bounds for bounded monotone sequences](error-bounds-for-bounded-monotone-sequences.md)

Even restricting to increasing [sequences](sequence.md) in $[0,1]$ with [limit of a sequence](limit-of-a-sequence.md) one gives no common stopping index. For any positive [integer](integer-split.md) $K$, define

$$
a_n=\begin{cases}0,&n\leq K,\\1-2^{-(n-K)},&n>K.\end{cases}
$$

This is an increasing [bounded sequence](bounded-sequence.md) converging to one, but its [absolute error](absolute-error.md) is one through index $K$. Since $K$ can exceed any proposed index, the [bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md) alone cannot say when the [absolute error](absolute-error.md) will fall below $1/2$. A zero difference between two successive terms is also insufficient: the initial plateau eventually ends.

There is no universal eventual rate either. Let $(r_n)$ be any proposed positive nonincreasing [sequence](sequence.md) tending to zero, with $r_n\leq1$. Set

$$
a_n=1-\sqrt{r_n}.
$$

Then $(a_n)$ is increasing, lies in $[0,1]$, and converges to one, but for every sufficiently large $n$ its [absolute error](absolute-error.md) satisfies $1-a_n=\sqrt{r_n}>r_n$. Indeed, $\sqrt{r_n}/r_n=1/\sqrt{r_n}\to\infty$, so no fixed constant multiple of $r_n$ bounds the [absolute error](absolute-error.md) eventually. If a proposed rate is not nonincreasing, replace it, after a finite initial segment if necessary, by the decreasing envelope $s_n=\sup\{r_k:k\geq n\}$; this also tends to zero, and the same construction defeats the original rate. This is an original construction, rather than a quantitative claim attributed to the qualitative theorem.

For a concrete slow example, $a_n=1-1/\log(n+2)$ increases to one, where $\log$ is the [natural logarithm](natural-logarithm.md). Its [absolute error](absolute-error.md) is $1/\log(n+2)$, so making it less than $\varepsilon$ requires $n+2>\exp(1/\varepsilon)$, using the [exponential function](exponential-function.md). At $\varepsilon=0.1$, this first happens at $n=22025$. The reciprocal and geometric examples in [increasing and decreasing approximations to a common limit](increasing-and-decreasing-approximations-to-a-common-limit.md) meet the same tolerance at $n=11$ and $n=4$, respectively. All three obey the same [bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md).

## ↑ Ancestors (10)

1. [Error bounds for bounded monotone sequences](error-bounds-for-bounded-monotone-sequences.md)
2. [Bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md)
3. [Monotone sequence](monotone-sequence.md)
4. [Sequence](sequence.md)
5. [Sequence and series](sequence-and-series-split.md)
6. [Real analysis](real-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)
