<h1 id="3f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonnegative integer-valued [random variable](../../../../../../random-variable-split.md) $X$, its [probability generating function](../../../../../../probability-generating-function.md) is

$$
G_X(z)=\mathbb E[z^X]=\sum_{k=0}^{\infty}\mathbb P(X=k)z^k,
$$

initially defined at least for $|z|\le1$. A general real-valued random variable need not have a [probability generating function](../../../../../../probability-generating-function.md) in this sense. For a [binomial distribution](../../../../../../binomial-distribution.md), the [binomial theorem](../../../../../../binomial-theorem.md) gives

$$
G_X(z)=\sum_{k=0}^n\binom nkp^k(1-p)^{n-k}z^k=(1-p+pz)^n.
$$

Differentiating the generating function produces factorial moments:

$$
\mathbb EX=G_X'(1)=np,\qquad
\mathbb E[X(X-1)]=G_X''(1)=n(n-1)p^2.
$$

Since $X^2=X(X-1)+X$, the [mean](../../../../../../expected-value.md) and [variance](../../../../../../variance-split.md) are

$$
\boxed{\mathbb EX=np,\qquad\operatorname{Var}(X)=np(1-p).}
$$

These formulas include the degenerate endpoint [probabilities](../../../../../../probability.md) and $n=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3F](../../3f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
