<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The given [relative Fisher information](../../../../../../relative-fisher-information.md) inequality is $I'(t)\leq-2I(t)$. Multiplying by $e^{2t}$ and integrating gives **[relative Fisher information decay under Ornstein-Uhlenbeck flow](../../../../../../relative-fisher-information-decay-under-ornstein-uhlenbeck-flow.md)**:

$$
\boxed{I(f_t\mid\gamma)\leq e^{-2(t-s)}I(f_s\mid\gamma)
\qquad(t\geq s\geq0).}
$$

In particular $I(t)\leq I(0)e^{-2t}$ when $I(0)$ is finite; if necessary one starts at a positive time with finite information. It follows that $I(t)\to0$.

Write $H(t)=H(f_t\mid\gamma)$. It is nonnegative and decreasing, so has a finite limit $H_\infty\geq0$ when $H(0)<\infty$. The printed integrability request concerns the product $H(t)H'(t)$. Its sign is nonpositive, and the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives

$$
\int_0^R|H(t)H'(t)|\,dt
=-\frac12\int_0^R(H(t)^2)'\,dt
=\frac{H(0)^2-H(R)^2}{2}.
$$

Passing to $R\to\infty$ proves **[time integrability of an entropy-dissipation product](../../../../../../time-integrability-of-an-entropy-dissipation-product.md)**:

$$
\boxed{H(t)H'(t)\in L^1(0,\infty),\qquad
\|HH'\|_{L^1}=\frac{H(0)^2-H_\infty^2}{2}\leq\frac{H(0)^2}{2}.}
$$

Also $\int_0^\infty|H'|=H(0)-H_\infty\leq H(0)$. The zero value of $H_\infty$ will be used as supplied in (f); positivity and monotonicity alone only establish existence of the limit.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
