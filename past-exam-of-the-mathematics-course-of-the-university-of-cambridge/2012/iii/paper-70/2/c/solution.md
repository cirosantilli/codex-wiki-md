<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First prove necessity. If [polynomials](../../../../../../polynomial-split.md) with [integer](../../../../../../integer.md) [coefficients](../../../../../../coefficient.md) converge to $f$ in the [supremum norm](../../../../../../supremum-norm.md), their values at $0$ and $1$ are convergent sequences of [integers](../../../../../../integer.md). Each such sequence is eventually constant, since a convergent sequence is [Cauchy](../../../../../../cauchy-sequence.md) and two distinct [integers](../../../../../../integer.md) are at distance at least one. Its limit is an [integer](../../../../../../integer.md). Thus $f(0),f(1)\in\mathbb Z$.

For sufficiency we also need [uniform convergence](../../../../../../uniform-convergence.md) of the [Bernstein polynomial](../../../../../../bernstein-polynomial.md) to $f$. Here is a direct argument. For $X\sim\operatorname{Bin}(n,x)$, write $B_n(f,x)=\mathbb E f(X/n)$. The [binomial distribution](../../../../../../binomial-distribution.md) has $\mathbb E(X/n)=x$ and $\operatorname{Var}(X/n)=x(1-x)/n\le1/(4n)$. For every $\delta>0$, [uniform continuity](../../../../../../uniform-continuity.md) of $f$ and the [Chebyshev inequality](../../../../../../chebyshev-inequality.md) give

$$
|B_n(f,x)-f(x)|\le\omega(f,\delta)+2\|f\|_\infty\mathbb P(|X/n-x|>\delta)
\le\omega(f,\delta)+\frac{\|f\|_\infty}{2n\delta^2}.
$$

First make $\delta$ small and then $n$ large; the bound is uniform in $x$. Hence $\|B_n(f)-f\|_\infty\to0$.

If the endpoints are [integers](../../../../../../integer.md), part (b) gives $\|B_n^*(f)-B_n(f)\|_\infty\to0$. Each coefficient multiplying $x^k(1-x)^{n-k}$ in $B_n^*$ is an [integer](../../../../../../integer.md). Expanding $(1-x)^{n-k}$ by the [binomial theorem](../../../../../../binomial-theorem.md) therefore gives [integer](../../../../../../integer.md) [coefficients](../../../../../../coefficient.md) in the ordinary monomial [basis](../../../../../../basis.md). The [triangle inequality](../../../../../../triangle-inequality.md) proves $\|B_n^*(f)-f\|_\infty\to0$. Thus **the [integer](../../../../../../integer.md) endpoint condition is necessary and sufficient** for [integer-coefficient polynomial approximation](../../../../../../integer-coefficient-polynomial-approximation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
