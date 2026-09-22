<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Define the [binomial coefficient](../../../../../binomial-coefficient.md) $\binom ni$ to be the number of $i$-element subsets of an $n$-element set. Counting ordered selections and dividing by the $i!$ orders of each subset gives

$$
\binom ni=\frac{n!}{i!(n-i)!},\qquad0\leq i\leq n.
$$

Every subset has exactly one size, while each of the $n$ elements can independently be included or omitted. Hence the [power set](../../../../../power-set.md) has $2^n$ members and

$$
\boxed{\sum_{i=0}^{n}\binom ni=2^n.}
$$

To prove the [binomial theorem](../../../../../binomial-theorem.md), expand the product of $n$ factors $(1+x)$. A term $x^i$ results from choosing $x$ from precisely an $i$-element subset of the factors and choosing one elsewhere. Its coefficient is therefore $\binom ni$. This is a finite distributive expansion, valid for every real $x$, and gives

$$
(1+x)^n=\sum_{i=0}^{n}\binom ni x^i.
$$

Differentiate this [polynomial identity](../../../../../polynomial-identity.md) and set $x=1$:

$$
\boxed{\sum_{i=0}^{n}i\binom ni=n2^{n-1}.}
$$

A second derivative gives $\sum i(i-1)\binom ni=n(n-1)2^{n-2}$ for $n\geq2$. Since $i^2=i(i-1)+i$, it follows that

$$
\boxed{\sum_{i=0}^{n}i^2\binom ni=n(n+1)2^{n-2}.}
$$

The formula also holds for $n=1$, when its value is one; that case can be checked directly without differentiating twice.

For the squared [binomial coefficients](../../../../../binomial-coefficient.md), compare the coefficient of $x^n$ in $(1+x)^n(1+x)^n=(1+x)^{2n}$. On the left it is $\sum_i\binom ni\binom n{n-i}$, and the [binomial coefficient](../../../../../binomial-coefficient.md) symmetry gives $\binom n{n-i}=\binom ni$. Thus

$$
\boxed{\sum_{i=0}^{n}\binom ni^2=\binom{2n}{n}.}
$$

Finally put $S=\sum_i i\binom ni^2$ and replace the index $i$ by $n-i$. The same symmetry gives $S=\sum_i(n-i)\binom ni^2$. Adding the two expressions and using the preceding identity yields

$$
\boxed{\sum_{i=0}^{n}i\binom ni^2=\frac n2\binom{2n}{n}.}
$$

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
