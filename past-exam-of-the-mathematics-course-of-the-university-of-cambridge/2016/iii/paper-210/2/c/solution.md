<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\ell=\log(d/\delta)$ and $r=\sqrt{\ell/n}\leq1$. Use the [quadratic scan statistic](../../../../../../quadratic-scan-statistic.md) $\Lambda$ and reject when $\Lambda>1+4r$. Under the [null hypothesis](../../../../../../null-hypothesis.md), each $n u(T)^\top\widehat\Sigma u(T)$ has the [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $n$ degrees of freedom. The [chi-squared concentration inequality](../../../../../../chi-squared-concentration-inequality.md) gives $P_0^{\otimes n}(\Lambda>1+2r+2r^2)\leq d e^{-\ell}=\delta$, by the [union bound](../../../../../../boole-s-inequality.md). Since $2r+2r^2\leq4r$, the proposed [Type I error](../../../../../../type-i-and-type-ii-errors.md) is at most $\delta$.

For the true set $S$, $n u(S)^\top\widehat\Sigma u(S)/(1+\theta)$ has the same [chi-squared distribution](../../../../../../chi-squared-distribution.md). We need a lower-tail bound that remains positive even when $\ell/n$ is close to one. Set $a=e^{-4r}$. The [chi-squared Chernoff lower-tail bound](../../../../../../chi-squared-chernoff-lower-tail-bound.md) gives $P(V\leq na)\leq\exp[-n(a-1-\log a)/2]\leq e^{-nr^2}=e^{-\ell}$: indeed $e^{-4r}-1+4r\geq2r^2$ for $0\leq r\leq1$. To verify this last inequality, its derivative is $4(1-r-e^{-4r})$; the expression in parentheses is strictly concave, starts at zero, and changes sign once, so the minimum occurs at an endpoint, where the inequality holds.

The function $g(r)=(1+4r)e^{4r}-1$ is [convex](../../../../../../convex-function.md) with $g(0)=0$, so $g(r)\leq r g(1)<300r$ on this interval. Consequently $\theta>300r$ implies $(1+\theta)e^{-4r}>1+4r$. Failure to reject then requires $V\leq na$, giving [Type II error](../../../../../../type-i-and-type-ii-errors.md) at most $e^{-\ell}\leq\delta$, uniformly in $S$. An explicit, deliberately conservative answer is

$$
\boxed{\psi=\mathbf1_{\{\Lambda>1+4\sqrt{\log(d/\delta)/n}\}},\qquad C=300.}
$$

The sharp constant is unnecessary; the detection scale is $\sqrt{\log(d/\delta)/n}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
