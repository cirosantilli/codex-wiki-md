# Coefficient recovery and factorial moments of a probability generating function

↑ **Parent:** [Probability generating function](probability-generating-function.md)

[Coefficient extraction](coefficient-extraction.md) recovers every [probability mass](probability-mass.md):

$$
p_k=\frac{G_X^{(k)}(0)}{k!},\qquad k=0,1,2,\ldots.
$$

Indeed, [termwise differentiation of a power series](termwise-differentiation-of-a-power-series.md) is valid inside $|s|<1$; evaluating the $k$th [derivative](derivative.md) at zero kills every term except $p_ks^k$. Thus two [probability generating functions](probability-generating-function.md) with the same [coefficients](coefficient.md) describe the same [probability distribution](probability-distribution-split.md), without any finite-[moment](moment.md) assumption.

At one, approach along the real line from below. For each positive integer $r$, [termwise differentiation of a power series](termwise-differentiation-of-a-power-series.md) followed by the [monotone convergence theorem](monotone-convergence-theorem.md) gives the [factorial moment](factorial-moment.md)

$$
G_X^{(r)}(1-):=\lim_{s\uparrow1}G_X^{(r)}(s)=\mathbb E[(X)_r],\qquad (X)_r=X(X-1)\cdots(X-r+1).
$$

For integer $X<r$, set $(X)_r=0$. The limit may be infinite; it is a finite boundary value only when the corresponding [factorial moment](factorial-moment.md) is finite. In particular, a finite first [moment](moment.md) gives

$$
\mathbb E[X]=G_X'(1-),
$$

and a finite second [moment](moment.md) gives

$$
\operatorname{Var}(X)=G_X''(1-)+G_X'(1-)-\bigl(G_X'(1-)\bigr)^2.
$$

The [variance](variance-split.md) formula follows from $X^2=X(X-1)+X$. These are boundary limits of [derivatives](derivative.md); they do not assert that the [probability generating function](probability-generating-function.md) extends smoothly through one.

For a nonnegative integer-valued [random variable](random-variable-split.md), its [moment-generating function](moment-generating-function.md) satisfies $M_X(t)=G_X(e^t)$ wherever finite. The guaranteed [probability generating function](probability-generating-function.md) domain therefore supplies finite values for real $t\leq0$; it does not guarantee positive [exponential moments](exponential-moment.md) or a finite [moment-generating function](moment-generating-function.md) on a neighborhood of zero. Bounded nonnegative integer-valued [random variables](random-variable-split.md) have polynomial [probability generating functions](probability-generating-function.md), but their convenient behavior is not a general existence theorem.

## ↑ Ancestors (7)

1. [Probability generating function](probability-generating-function.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
