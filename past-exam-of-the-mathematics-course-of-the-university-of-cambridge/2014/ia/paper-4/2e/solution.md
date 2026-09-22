<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

For [integers](../../../../../integer.md) $0\leq k\leq n$, define the [binomial coefficient](../../../../../binomial-coefficient.md) by

$$
\binom nk=\frac{n!}{k!(n-k)!},\qquad0!=1.
$$

Here the [factorial](../../../../../factorial.md) $n!$ is the product of the positive [integers](../../../../../integer.md) up to $n$. This also counts the $k$-element [subsets](../../../../../subset.md) of an $n$-element [set](../../../../../set-split.md): an ordered choice has $n!/(n-k)!$ possibilities, and each [subset](../../../../../subset.md) is ordered in $k!$ ways.

Directly from the [factorial](../../../../../factorial.md) definition, when $0\leq k<n$,

$$
\binom nk+\binom n{k+1}
=\frac{n!(k+1)+n!(n-k)}{(k+1)!(n-k)!}
=\frac{(n+1)!}{(k+1)!(n-k)!}
=\boxed{\binom{n+1}{k+1}}.
$$

This is [Pascal's identity](../../../../../pascal-s-rule.md).

The required [hockey-stick identity](../../../../../hockey-stick-identity.md) follows by [mathematical induction](../../../../../mathematical-induction.md) on $m$, with $n\geq0$ fixed. For $m=0$, both sides are $1$. If it holds at $m$, adding the next [binomial coefficient](../../../../../binomial-coefficient.md) and using [Pascal's identity](../../../../../pascal-s-rule.md) gives

$$
\sum_{k=0}^{m+1}\binom{n+k}k
=\binom{n+m+1}m+\binom{n+m+1}{m+1}
=\binom{n+m+2}{m+1}.
$$

Therefore **for every $n,m\geq0$**,

$$
\boxed{\sum_{k=0}^m\binom{n+k}k=\binom{n+m+1}m.}
$$

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
