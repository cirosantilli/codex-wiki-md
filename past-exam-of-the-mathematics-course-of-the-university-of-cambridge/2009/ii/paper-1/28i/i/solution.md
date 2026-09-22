<h1 id="28i/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The joint [likelihood](../../../../../../likelihood-function.md) is $\lambda^n e^{-\lambda T_n}\prod_i\mathbf1_{x_i>0}$, so the [factorization criterion for sufficiency](../../../../../../fisher-neyman-factorization-theorem.md) proves sufficiency. For any two positive sample vectors its likelihood ratio is $e^{-\lambda(T_n(x)-T_n(y))}$, independent of $\lambda$ exactly when their sums agree. The [likelihood-ratio criterion for minimal sufficiency](../../../../../../likelihood-ratio-criterion-for-minimal-sufficiency.md) therefore makes $T_n$ minimal sufficient.

Its [gamma distribution](../../../../../../gamma-distribution.md) has density $\lambda^nt^{n-1}e^{-\lambda t}/\Gamma(n)$ on $t>0$. If $g(T_n)$ is integrable for every $\lambda$ and has expectation zero for every $\lambda$, then

$$
\int_0^\infty g(t)t^{n-1}e^{-\lambda t}\,dt=0\qquad(\lambda>0).
$$

By uniqueness of the [Laplace transform](../../../../../../laplace-transform.md), $g(t)t^{n-1}=0$ almost everywhere. One may first multiply by $e^{-\lambda_0t}$ to obtain an integrable function and use transform parameters $\lambda>\lambda_0$; this handles the transform's integrability hypothesis. Since the gamma densities are positive on $(0,\infty)$, $g(T_n)=0$ almost surely for every $\lambda$. **$T_n$ is complete as well as minimal sufficient.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [28I](../../28i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
