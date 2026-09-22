<h1 id="9d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $r=e^{i\theta}\ne1$. The [geometric series](../../../../../../geometric-series.md) from any starting index is bounded:

$$
B_j=\sum_{n=m}^j r^n=\frac{r^m(1-r^{j-m+1})}{1-r},\qquad
|B_j|\leq K=\frac2{|1-r|}.
$$

Using [summation by parts](../../../../../../abel-s-summation-formula.md),

$$
\sum_{n=m}^N a_nr^n=a_NB_N+\sum_{n=m}^{N-1}(a_n-a_{n+1})B_n.
$$

Since the coefficients are nonincreasing and positive, the [modulus](../../../../../../modulus.md) is at most $K(a_N+a_m-a_N)=Ka_m\to0$. The Cauchy criterion proves **convergence for every $\theta\notin2\pi\mathbb Z$**. This is a direct proof of the [Dirichlet test](../../../../../../dirichlet-test.md) in this setting.

For $a_n=1/n$, the imaginary parts of the convergent partial sums give convergence of the sine series at those angles. If $\theta\in2\pi\mathbb Z$, every sine term is zero. Hence **the sine series converges for all real angles**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9D](../../9d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
