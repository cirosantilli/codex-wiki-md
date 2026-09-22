<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Hoeffding inequality](../../../../../hoeffding-inequality.md) states that if $X_1,\ldots,X_n$ are [independent random variables](../../../../../independent-random-variables.md) with $a_i\leq X_i\leq b_i$ almost surely, then for $t>0$

$$
P\left(\sum_{i=1}^n(X_i-EX_i)\geq t\right)\leq\exp\left(-\frac{2t^2}{\sum_i(b_i-a_i)^2}\right).
$$

The same bound holds for the lower tail. Consequently the two-sided tail is at most twice this bound. When all ranges have length zero, the sum is deterministic and every positive tail probability is zero.

We construct an [exponential packing of a Hamming cube](../../../../../exponential-packing-of-a-hamming-cube.md). Choose an [inclusion-maximal separated set](../../../../../inclusion-maximal-separated-set.md) $S$ in $\{-1,1\}^n$ with separation at least $r=n/8$ for the [Hamming distance](../../../../../hamming-distance.md). It exists by a finite greedy procedure: keep adding any vertex at distance at least $r$ from all selected vertices until none remains. By maximality, every vertex is within distance strictly less than $r$ of some member of $S$. This is the principle that [maximal separated sets give covers](../../../../../maximal-separated-sets-give-covers.md).

For a uniformly random vertex $U$ and any fixed vertex $s$, the mismatch indicators in different coordinates are [independent](../../../../../independent-random-variables.md) [Bernoulli random variables](../../../../../bernoulli-distribution.md) with success probability $1/2$. Hence $\rho(U,s)$ has the [binomial distribution](../../../../../binomial-distribution.md) with parameters $n,1/2$. The lower-tail [Hoeffding inequality](../../../../../hoeffding-inequality.md) gives

$$
P\left(\rho(U,s)\leq\frac n8\right)=P\left(\rho(U,s)-\frac n2\leq-\frac{3n}8\right)\leq e^{-9n/32}.
$$

Thus the [Hoeffding lower-tail bound for Hamming balls](../../../../../hoeffding-lower-tail-bound-for-hamming-balls.md) shows that every strict-radius ball $B_{<r}(s)$ has at most $2^ne^{-9n/32}$ vertices. Using a strict ball handles noninteger $n/8$ without changing the required separation.

The strict balls centered at $S$ cover the entire [Hamming cube](../../../../../hamming-cube.md). Counting their union by the sum of their sizes yields

$$
2^n\leq\sum_{s\in S}|B_{<r}(s)|\leq|S|\,2^ne^{-9n/32},\qquad |S|\geq e^{9n/32}\geq e^{n/4}.
$$

Therefore

$$
\boxed{|S|\geq e^{n/4},\qquad\min_{s\ne s'\in S}\rho(s,s')\geq n/8.}
$$

In particular this proves the assertion for every $n\geq8$. Maximality here means that no further vertex can be added; finding a largest [separated set](../../../../../separated-subset-of-a-metric-space.md) is unnecessary.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 36](../../paper-36-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
