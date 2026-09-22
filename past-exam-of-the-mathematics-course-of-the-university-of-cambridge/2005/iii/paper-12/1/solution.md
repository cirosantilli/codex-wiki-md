<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $N=\sum_{i=1}^n\mathbf1_{E_i}$, and put $S_0=1$, $S_j=\sum_{|I|=j}\Pr(\bigcap_{i\in I}E_i)$ for $j\ge1$. Counting the $j$-subsets of the events that occur gives $S_j=\mathbb E\binom Nj$. Set $S_j=0$ for $j>n$. The [Jordan-Bonferroni exact-occurrence inequalities](../../../../../jordan-bonferroni-exact-occurrence-inequalities.md) are

$$
\boxed{\sum_{r=0}^{2s+1}(-1)^r\binom{k+r}kS_{k+r}\le\Pr(N=k)\le\sum_{r=0}^{2s}(-1)^r\binom{k+r}kS_{k+r}\quad(s\ge0).}
$$

Here $k\ge0$ is an integer. To prove both bounds, evaluate the truncated expression before taking its [expectation](../../../../../expected-value.md). At an integer value $N=j\ge k$ it equals

$$
\binom jk\sum_{r=0}^m(-1)^r\binom{j-k}r.
$$

For $j=k$ this is one. For $j>k$, [Pascal's identity](../../../../../pascal-s-rule.md), or an induction on $m$, gives

$$
\sum_{r=0}^m(-1)^r\binom{j-k}r=\begin{cases}(-1)^m\binom{j-k-1}m,&m<j-k,\\0,&m\ge j-k.\end{cases}
$$

For $j<k$ the original expression is zero. Thus its difference from $\mathbf1_{\{N=k\}}$ is everywhere nonnegative for even $m$ and nonpositive for odd $m$. Taking [expectations](../../../../../expected-value.md) proves the inequalities, including $k=0$.

For a general nonnegative integer-valued [random variable](../../../../../random-variable-split.md), define its [factorial moment](../../../../../factorial-moment.md) by $\mathbb E_r(X)=\mathbb E(X)_r$, where $(X)_r$ is the [falling factorial](../../../../../falling-factorial.md) and $\mathbb E_0(X)=1$. The same pointwise calculation applies to $X$, so put

$$
T_m=\frac1{k!}\sum_{r=0}^m\frac{(-1)^r\mathbb E_{k+r}(X)}{r!}.
$$

Every required moment is finite under the given limit assumption: eventual finiteness of higher [factorial moments](../../../../../factorial-moment.md) implies finiteness of the lower ones. The neighbouring upper and lower bounds differ in absolute value by

$$
|T_{m+1}-T_m|=\frac{\mathbb E_{k+m+1}(X)}{k!(m+1)!}=\frac1{k!}\frac{\mathbb E_s(X)s^k}{s!}\frac{(s)_k}{s^k},\qquad s=k+m+1.
$$

The last ratio tends to one, and the first factor involving the moment tends to zero. Since $\Pr(X=k)$ lies between every two such neighbouring bounds, each $T_m$ tends to it. Consequently the [factorial-moment inversion](../../../../../factorial-moment-inversion.md) is

$$
\boxed{\Pr(X=k)=\frac1{k!}\sum_{r=0}^\infty\frac{(-1)^r\mathbb E_{k+r}(X)}{r!}.}
$$

This proves convergence of the signed [series](../../../../../series-mathematics.md) without an unjustified interchange with an [expectation](../../../../../expected-value.md).

For any prescribed $r\ge1$, take $\Pr(X=j)=C_rj^{-(r+2)}$ for $j=1,2,\ldots$, with $C_r=[\sum_{j\ge1}j^{-(r+2)}]^{-1}$. Since $(j)_r\sim j^r$ and $(j)_{r+1}\sim j^{r+1}$, the two moment sums have tails comparable respectively to $\sum j^{-2}$ and $\sum j^{-1}$. Thus **$\mathbb E_r(X)<\infty$ but $\mathbb E_{r+1}(X)=\infty$**, as required.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
