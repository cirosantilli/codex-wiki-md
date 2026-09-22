<h1 id="12/solution">Solution</h1>

↑ **Parent:** [12](../12.md)

For [finite sets](../../../../../finite-set.md) $A_1,\ldots,A_n$, the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) states

$$
\boxed{\left|\bigcup_{i=1}^n A_i\right|
=\sum_{\varnothing\ne J\subseteq\{1,\ldots,n\}}
(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.}
$$

To prove it, fix an element in exactly $r$ of the [sets](../../../../../set-split.md). If $r=0$, it contributes to neither side. If $r\geq1$, its contribution to the right side is

$$
\sum_{k=1}^r(-1)^{k+1}\binom rk
=1-(1-1)^r=1,
$$

using the [binomial theorem](../../../../../binomial-theorem.md). This is exactly its contribution to the union. Summing over the finite ambient union proves the formula. Equivalently, the proof is an identity of elementwise membership indicators, so no unproved rule for overlapping sets is being assumed.

Now let the ambient [set](../../../../../set-split.md) be all $n!$ [permutations](../../../../../permutation.md), and let $E_i$ be those fixing element $i$. A [set intersection](../../../../../set-intersection.md) of $k$ specified events $E_i$ has $(n-k)!$ elements: the specified elements are fixed and the others may be permuted freely. Apply [inclusion-exclusion](../../../../../inclusion-exclusion-principle.md) to the complement of the union of these events. There are $\binom nk$ possible choices of the fixed positions, hence the [derangement](../../../../../derangement-of-a-permutation.md) count is

$$
\begin{aligned}
f(n)&=\sum_{k=0}^n(-1)^k\binom nk(n-k)!\\
&=\boxed{n!\sum_{k=0}^n\frac{(-1)^k}{k!}}.
\end{aligned}
$$

The $k=0$ term counts the whole ambient [set](../../../../../set-split.md) before subtraction; it is not an omitted empty intersection. The formula also gives $f(0)=1$ and $f(1)=0$.

Dividing by the [factorial](../../../../../factorial.md) and using the convergent power series for the [exponential function](../../../../../exponential-function.md) at $-1$ gives

$$
\boxed{\lim_{n\to\infty}\frac{f(n)}{n!}=\sum_{k=0}^\infty\frac{(-1)^k}{k!}=e^{-1}.}
$$

The alternating-series estimate supplies the explicit error bound $|f(n)/n!-e^{-1}|\leq1/(n+1)!$. Thus the limiting proportion is established, not merely identified from the first few values.

## ↑ Ancestors (10)

1. [12](../12.md)
2. [Paper 5](../../paper-5-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
