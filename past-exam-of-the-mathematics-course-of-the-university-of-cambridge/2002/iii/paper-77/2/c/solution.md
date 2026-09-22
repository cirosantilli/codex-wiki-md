<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $n$ fixed, the asymptotic family is the scaled sum

$$
S^L=\frac{X_1+\cdots+X_n}{L},\qquad L\to\infty.
$$

An unscaled fixed random variable alone has no diverging parameter for a [large deviation principle](../../../../../../large-deviation-principle.md); this scaling is the continuation of part (a). Suppose first $0<p_i<1$ and put $a_i=-\log(1-p_i)$. [Independence](../../../../../../independent-random-variables.md) and the [product large-deviation principle](../../../../../../product-large-deviation-principle.md) give the vector $(X_1/L,\ldots,X_n/L)$ rate

$$
I(x_1,\ldots,x_n)=
\begin{cases}
\sum_{i=1}^na_ix_i,&x_i\geq0\ \text{for every }i,\\
+\infty,&\text{otherwise}.
\end{cases}
$$

Addition is [continuous](../../../../../../continuous-function.md), so the [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) gives

$$
J(s)=\inf_{\substack{x_i\geq0\\\sum_i x_i=s}}\sum_i a_ix_i.
$$

For $s\geq0$ every feasible vector has cost at least $s a_*$, where $a_*=\min_i a_i$. Equality holds by assigning all scaled excess to an index attaining $a_*$. For $s<0$ the constraint set is empty. Thus

$$
\boxed{J(s)=
\begin{cases}
s\min_i[-\log(1-p_i)],&s\geq0,\\
+\infty,&s<0,
\end{cases}\qquad\text{speed }L.}
$$

Equivalently, the coefficient is $-\log(1-p_*)$ with $p_*=\min_i p_i$. On the exponential scale the rare large sum is carried by a variable having the slowest geometric tail. Several equal slowest tails can change polynomial prefactors, but not this [rate function](../../../../../../rate-function.md). This is the [large deviations of a fixed sum of geometric random variables](../../../../../../large-deviations-of-a-fixed-sum-of-geometric-random-variables.md).

As a direct check of the tail exponent, for each $0<\theta<a_*$ the [moment-generating function](../../../../../../moment-generating-function.md) of the sum is finite, so the [Chernoff bound](../../../../../../chernoff-bound.md) gives an upper rate at most $-\theta s$ for $s>0$. Letting $\theta\uparrow a_*$ gives $-a_*s$. For a lower neighborhood bound, keep all other variables at fixed finite values and let a slowest-tail variable take an integer near $Ls$; its probability has rate $-a_*s$. If some $p_i=1$, their deterministic contributions disappear after division by $L$, so minimize over the nondeterministic variables. If all $p_i=1$, the rate is zero only at zero and infinite elsewhere.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
