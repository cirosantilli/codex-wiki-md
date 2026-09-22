<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Set $m=\lceil p/100\rceil$ and $d=m-1$, so that $d<p/100<p$. The [dimension of a bounded-total-degree polynomial space](../../../../../dimension-of-a-bounded-total-degree-polynomial-space.md) in $n$ variables over $\mathbb F_p$ is $\binom{n+d}{n}$. If $\#N$ were smaller than this dimension, evaluation at the points of $N$ would impose fewer homogeneous linear conditions than unknown coefficients. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) would give a nonzero [multivariate polynomial](../../../../../multivariate-polynomial.md) $P$ of [total degree](../../../../../total-degree-of-a-polynomial.md) at most $d$, vanishing on $N$.

For every $x$, select one of the promised rich [affine lines in a vector space](../../../../../affine-line-in-a-vector-space.md) through $x$, and write it as $\ell=\{a+tv:t\in\mathbb F_p\}$ with $v\ne0$. The [polynomial restriction to a line](../../../../../polynomial-restriction-to-a-line.md) $Q(t)=P(a+tv)$ has degree at most $d$, and at least $m=d+1$ distinct [roots of a polynomial](../../../../../root-of-a-polynomial.md) from $N\cap\ell$. By the [root bound for a polynomial](../../../../../lagrange-root-bound-over-a-field.md), **$Q$ is identically zero**, so $P(x)=0$. Since this works for every $x$, $P$ vanishes at all $p^n$ points of $\mathbb F_p^n$.

The [Schwartz-Zippel lemma](../../../../../schwartz-zippel-lemma.md) says that a nonzero [multivariate polynomial](../../../../../multivariate-polynomial.md) of [total degree](../../../../../total-degree-of-a-polynomial.md) $d$ has at most $d p^{n-1}$ zeros on this grid. Here $d<p$, so that count is strictly less than $p^n$, a contradiction. The distinction between a formal [polynomial](../../../../../polynomial-split.md) and its function on a [finite field](../../../../../finite-field.md) is crucial: our degree bound is what rules out a nonzero [polynomial](../../../../../polynomial-split.md) vanishing everywhere.

We have proved the stronger quantitative [rich line covering bound over a finite field](../../../../../rich-line-covering-bound-over-a-finite-field.md)

$$
\boxed{\#N\ge\binom{n+\lceil p/100\rceil-1}{n}
=\frac{(d+1)\cdots(d+n)}{n!}
\ge\frac{p^n}{100^n n!}.}
$$

Thus **$\#N\gtrsim_n p^n$**, as required. The implied constant may depend on the fixed dimension $n$. The very large numerical lower bound on $p$ is more than this proof needs.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
