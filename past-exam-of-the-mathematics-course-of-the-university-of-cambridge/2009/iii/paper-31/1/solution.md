<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $a<b$, let $U_N[a,b]$ be the number of completed [upcrossings](../../../../../upcrossing.md) by the observations $X_1,\ldots,X_N$: buy when the value is at most $a$, sell at the first subsequent value at least $b$, and repeat. With $z^-=\max\{-z,0\}$, one form of the [Doob upcrossing inequality](../../../../../doob-upcrossing-inequality.md) for a [martingale](../../../../../martingale-split.md) is

$$
(b-a)\mathbb E U_N[a,b]\le\mathbb E(X_N-a)^-.
$$

For completeness, hold either zero or one unit according to this rule. The holding at each step is measurable before the next [martingale](../../../../../martingale-split.md) increment, so the total gain $G_N$ has [expected value](../../../../../expected-value.md) zero. Completed trades earn at least $b-a$ each; an unfinished trade loses at most $(X_N-a)^-$. Thus $G_N\ge(b-a)U_N[a,b]-(X_N-a)^-$, proving the inequality.

Suppose $C=\sup_n\mathbb E|X_n|<\infty$. For each rational pair $a<b$ the inequality and [monotone convergence](../../../../../monotone-convergence-theorem.md) give

$$
\mathbb E U_\infty[a,b]\le\frac{C+|a|}{b-a}<\infty.
$$

Every rational interval therefore has only finitely many [upcrossings](../../../../../upcrossing.md), simultaneously outside a countable union of null sets. If $\liminf X_n<\limsup X_n$, there is a rational interval strictly between them and infinitely many [upcrossings](../../../../../upcrossing.md), a contradiction. Thus the limit $X_\infty$ exists in the extended real line [almost surely](../../../../../almost-sure-convergence.md). [Fatou's lemma](../../../../../fatou-s-lemma.md) now gives

$$
\mathbb E|X_\infty|\le\liminf_n\mathbb E|X_n|\le C.
$$

The limit is finite [almost surely](../../../../../almost-sure-convergence.md) and integrable. This proves the [martingale convergence theorem](../../../../../martingale-convergence-theorem.md) rather than using it as the deduction.

The exact extra condition for [convergence in L1](../../../../../convergence-in-l1.md) is **[uniform integrability](../../../../../uniform-integrability.md)**:

$$
\boxed{\lim_{K\to\infty}\sup_n\mathbb E\bigl[|X_n|\mathbf1_{\{|X_n|>K\}}\bigr]=0.}
$$

To see sufficiency, first discard the tails of $X_n$ uniformly and the tail of the integrable $X_\infty$. On the set where both absolute values are at most $K$, their difference is bounded by $2K$ and tends to zero [almost surely](../../../../../almost-sure-convergence.md); [dominated convergence](../../../../../dominated-convergence-theorem.md) finishes the proof. Conversely, if $X_n\to X_\infty$ in $L^1$, then

$$
\mathbb E\bigl[|X_n|\mathbf1_{\{|X_n|>K\}}\bigr]\le2\mathbb E|X_n-X_\infty|+\mathbb E\bigl[|X_\infty|\mathbf1_{\{|X_\infty|>K/2\}}\bigr].
$$

Make the first term uniformly small for all sufficiently large $n$, then control the finitely many remaining integrable variables by increasing $K$. Hence [uniform integrability](../../../../../uniform-integrability.md) is necessary too. In this case the [conditional expectation](../../../../../conditional-expectation.md) identity $X_n=\mathbb E[X_\infty\mid\mathcal F_n]$ follows by taking the $L^1$ limit in $X_n=\mathbb E[X_m\mid\mathcal F_n]$ for $m\ge n$.

The [coin-doubling martingale](../../../../../coin-doubling-martingale.md) shows why an $L^1$ bound is not enough. Let $\xi_1,\xi_2,\ldots$ be independent fair coin indicators and set

$$
X_n=2^n\mathbf1_{\{\xi_1=\cdots=\xi_n=1\}}.
$$

Conditional on the first $n$ coins, the next value is either $2X_n$ or zero with equal [probabilities](../../../../../probability.md), so this is a nonnegative [martingale](../../../../../martingale-split.md). Its [expected value](../../../../../expected-value.md) is always $1$, while a first failure occurs [almost surely](../../../../../almost-sure-convergence.md), giving $X_n\to0$ [almost surely](../../../../../almost-sure-convergence.md). Yet $\mathbb E|X_n-0|=1$ for every $n$. Indeed, whenever $2^n>K$, its tail [expected value](../../../../../expected-value.md) above $K$ is still $1$. Thus **[convergence in L1](../../../../../convergence-in-l1.md) fails because [uniform integrability](../../../../../uniform-integrability.md) fails**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
