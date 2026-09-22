# Error bounds for bounded monotone sequences

↑ **Parent:** [Bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md)

For an increasing [sequence](sequence.md) converging to $L$, its [absolute error](absolute-error.md) is $e_n=L-a_n\geq0$ and is nonincreasing. For a decreasing [sequence](sequence.md), the [absolute error](absolute-error.md) is $e_n=a_n-L\geq0$ and is also nonincreasing. This tells us that later terms cannot be worse, but does not supply a computable stopping index for a chosen tolerance.

Suppose an increasing lower approximation $a_n$ and a decreasing upper approximation $b_n$ enclose the same [limit of a sequence](limit-of-a-sequence.md) $L$. Their observable gap $w_n=b_n-a_n$ gives

$$
a_n\leq L\leq b_n\quad\Longrightarrow\quad
|a_n-L|\leq w_n,\qquad |b_n-L|\leq w_n,\qquad
\left|\frac{a_n+b_n}{2}-L\right|\leq\frac{w_n}{2}.
$$

If $w_n\to0$, the [squeeze theorem](squeeze-theorem.md) certifies a common [limit of a sequence](limit-of-a-sequence.md); the midpoint has a certified [absolute error](absolute-error.md) at most half the gap. This is the principle behind the [bisection method](bisection-method.md). In the symmetric example $a_n=1-1/n$, $b_n=1+1/n$, the gap is $2/n$, each endpoint's exact [absolute error](absolute-error.md) is $1/n$, and the midpoint happens to equal one exactly. The bound is valid even when such symmetry is absent.

A fixed [upper bound](upper-bound-in-a-partially-ordered-set.md) by itself supplies less. If $a_n\uparrow L$ and $a_n\leq M$ for all $n$, then $L\leq M$ and $0\leq L-a_n\leq M-a_n$, but the last gap need not vanish. Taking $a_n=1-1/n$ and $M=2$ makes $M-a_n\to1$. A shrinking bracket or an explicit remainder formula adds information that qualitative convergence does not provide.

**Table of contents**

- [Bounded monotone sequences have no universal convergence rate](bounded-monotone-sequences-have-no-universal-convergence-rate.md)

## ↑ Ancestors (9)

1. [Bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md)
2. [Monotone sequence](monotone-sequence.md)
3. [Sequence](sequence.md)
4. [Sequence and series](sequence-and-series-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md)
