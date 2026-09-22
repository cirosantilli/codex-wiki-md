<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

For a nonnegative integer-valued [random variable](../../../../../random-variable-split.md), the [probability generating function](../../../../../probability-generating-function.md) is

$$
G_X(s)=\mathbb E[s^X]=\sum_{j=0}^\infty P(X=j)s^j,
$$

with $0\leq s\leq1$ always allowed. Its derivative at $1$ from below gives the [expectation](../../../../../expected-value.md) when finite.

The waiting time $N$ has the positive-integer [geometric distribution](../../../../../geometric-distribution.md) $P(N=j)=pq^{j-1}$. For the [capped geometric waiting time](../../../../../capped-geometric-waiting-time.md), $X=j<k$ exactly when $N=j$, while $X=k$ occurs whenever $N\geq k$. Thus the terminal mass is $q^{k-1}$, giving

$$
\boxed{G_X(s)=p\sum_{j=1}^{k-1}q^{j-1}s^j+q^{k-1}s^k
=\frac{ps+q^ks^k(1-s)}{1-qs}}.
$$

The finite sum is a polynomial; any apparent singularity of the rational expression is removable. This includes $k=1$, where $G_X(s)=s$.

Differentiating the rational form at $s=1$ yields

$$
G_X'(1)=\frac{(p-q^k)p+pq}{p^2}=\boxed{\frac{1-q^k}{p}}.
$$

As a second interpretation, the [expectation](../../../../../expected-value.md) is the sum of the tail [probabilities](../../../../../probability.md) $P(X\geq j)=q^{j-1}$ for $1\leq j\leq k$. Their finite geometric sum gives the same answer.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
