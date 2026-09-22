<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [hitting time](../../../../../../first-passage-time.md) $T$ is a [stopping time](../../../../../../stopping-time.md) for the [natural filtration](../../../../../../natural-filtration.md), because $\{T\leq n\}=\bigcup_{k\leq n}\{S_k=b\}$. The integer-valued increments are at most one. A path started at zero therefore cannot reach or exceed $b$ without first visiting $b$, so

$$
S_{n\wedge T}\leq b\quad\text{for every }n.
$$

Define $Y_n=b-S_{n\wedge T}$. It is nonnegative and integrable: $|S_{n\wedge T}|\leq\sum_{j\leq n}|X_j|$. Moreover,

$$
S_{(n+1)\wedge T}-S_{n\wedge T}=\mathbf1_{\{T>n\}}X_{n+1}.
$$

The [indicator function](../../../../../../indicator-function.md) is $\mathcal F_n$-measurable, and $X_{n+1}$ is independent of $\mathcal F_n$ with zero [expected value](../../../../../../expected-value.md). Taking [conditional expectation](../../../../../../conditional-expectation.md) therefore proves directly that $(Y_n)$ is a nonnegative [martingale](../../../../../../martingale-split.md).

The general result used here is that a nonnegative discrete-time [martingale](../../../../../../martingale-split.md) has a finite almost-sure limit; this is the [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md), since $\mathbb E Y_n=\mathbb E Y_0=b$ bounds its [L1 norm](../../../../../../l1-norm.md). On $\{T=\infty\}$ it follows that $S_n=b-Y_n$ converges finitely. A convergent sequence of integers is eventually constant, so $X_n=S_n-S_{n-1}$ would eventually be zero on this [event](../../../../../../event.md).

However, the independent [events](../../../../../../event.md) $\{X_n=1\}$ all have the same strictly positive [probability](../../../../../../probability.md). The second [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md) says that they occur infinitely often [almost surely](../../../../../../almost-sure-convergence.md). This contradicts eventual constancy on any positive-probability subset of $\{T=\infty\}$. Thus

$$
\boxed{\mathbb P(T<\infty)=1.}
$$

Notice that no lower bound on the negative increments was needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
