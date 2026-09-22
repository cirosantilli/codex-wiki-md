# Discrete uniform moments on an integer interval

↑ **Parent:** [Discrete uniform distribution](discrete-uniform-distribution.md)

Suppose the [support of a probability distribution](support-of-a-probability-distribution.md) consists of all consecutive [integers](integer-split.md) from $a$ to $b$, including both endpoints, with $a\leq b$. Its [cardinality](cardinality.md) is $n=b-a+1$, and a [discrete uniform distribution](discrete-uniform-distribution.md) on it satisfies

$$
\mathbb E X=\frac{a+b}{2},\qquad
\operatorname{Var}(X)=\frac{n^2-1}{12}=\frac{(b-a)(b-a+2)}{12}.
$$

For a short derivation, set $K=X-a$, whose possible values are $0,\ldots,n-1$. The finite [sums](sum.md) give

$$
\sum_{k=0}^{n-1}k=\frac{n(n-1)}2,\qquad
\sum_{k=0}^{n-1}k^2=\frac{n(n-1)(2n-1)}6,
$$

and hence

$$
\mathbb E K=\frac{n-1}{2},\qquad
\mathbb E[K^2]=\frac{(n-1)(2n-1)}6,\qquad
\operatorname{Var}(K)=\frac{(n-1)(2n-1)}6-\frac{(n-1)^2}{4}=\frac{n^2-1}{12}.
$$

Adding $a$ shifts the [expected value](expected-value-split.md) by $a$ and leaves the [variance](variance-split.md) unchanged. For completeness, the first [sum](sum.md) follows by pairing $k$ with $n-1-k$. For the second, sum $(k+1)^3-k^3=3k^2+3k+1$ from $k=0$ to $n-1$: the left side is $n^3$, so inserting the first [sum](sum.md) gives the stated result.

The edge case $a=b$ has $n=1$: $X=a$ with [probability](probability.md) one, [expected value](expected-value-split.md) $a$, and [variance](variance-split.md) zero. On an [arithmetic progression](arithmetic-progression.md) $\{a,a+h,\ldots,a+(n-1)h\}$ with $h>0$, the same argument instead gives [expected value](expected-value-split.md) $a+h(n-1)/2$ and [variance](variance-split.md) $h^2(n^2-1)/12$. Equal spacing is the extra hypothesis behind these formulas; the [discrete uniform distribution](discrete-uniform-distribution.md) on $\{1,2,4,8\}$ requires the general [sums](sum.md) above.

## ↑ Ancestors (8)

1. [Discrete uniform distribution](discrete-uniform-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
