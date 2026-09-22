<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If [polynomials](../../../../../../polynomial-split.md) with [integer](../../../../../../integer.md) monomial [coefficients](../../../../../../coefficient.md) converge uniformly to $f$, their values at zero and one are [integers](../../../../../../integer.md) converging to $f(0)$ and $f(1)$. A convergent [integer](../../../../../../integer.md) sequence is eventually constant: once all its terms lie in an interval of length less than one they must agree. Hence both endpoint values are [integers](../../../../../../integer.md).

Conversely assume those values are [integers](../../../../../../integer.md). The [rounded Bernstein polynomial](../../../../../../rounded-bernstein-polynomial.md) is an [integer](../../../../../../integer.md)-[coefficient](../../../../../../coefficient.md) [polynomial](../../../../../../polynomial-split.md), because its displayed scalar [coefficients](../../../../../../coefficient.md) are [integers](../../../../../../integer.md) and each $x^k(1-x)^{n-k}$ expands with [integer](../../../../../../integer.md) [coefficients](../../../../../../coefficient.md). Part b gives its vanishing distance from $B_nf$. For completeness, the remaining [uniform convergence](../../../../../../uniform-convergence.md) $B_nf\to f$ follows directly from [uniform continuity](../../../../../../uniform-continuity.md). Let $X$ have the [binomial distribution](../../../../../../binomial-distribution.md) with parameters $n,x$; then $B_n(f,x)=\mathbb E f(X/n)$, $\mathbb E(X/n)=x$, and $\operatorname{Var}(X/n)=x(1-x)/n\le1/(4n)$. Splitting into $|X/n-x|\le\delta$ and its complement, and applying [Chebyshev's inequality](../../../../../../chebyshev-inequality.md), gives

$$
|B_n(f,x)-f(x)|\le\omega(f,\delta)+2\|f\|_\infty\frac1{4n\delta^2},
$$

where $\omega$ is the [modulus of continuity](../../../../../../modulus-of-continuity.md). First choose $\delta$ to make the first term small uniformly, then take $n$ large. The [triangle inequality](../../../../../../triangle-inequality.md) now gives $\|B_n^*f-f\|_\infty\to0$. We have proved the [integer-coefficient polynomial approximation](../../../../../../integer-coefficient-polynomial-approximation.md) characterization

$$
\boxed{f\in\overline{\mathbb Z[x]}^{\|\cdot\|_\infty}
\quad\Longleftrightarrow\quad f(0),f(1)\in\mathbb Z.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
