<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $f=(f(x_1),\ldots,f(x_n))^T$, so $Y=f+\varepsilon$ and $Y^*=f+\varepsilon^*$ with independent noise vectors having [covariance matrix](../../../../../../covariance-matrix.md) $I_n$. For any deterministic [linear smoother](../../../../../../linear-smoother.md) $H$,

$$
\mathbb E\|Y-HY\|_2^2
=\|(I-H)f\|_2^2
+\operatorname{tr}\!\left((I-H)^T(I-H)\right),
$$

whereas independence gives

$$
\mathbb E\|Y^*-HY\|_2^2
=\|(I-H)f\|_2^2+n+\operatorname{tr}(H^TH).
$$

Expanding the first trace shows that the second expression exceeds the first by $2\operatorname{tr}(H)$, proving the identity.

For ridge regression,

$$
H_\lambda=\frac1n\mathbf1\mathbf1^T
+X(X^TX+\lambda I_p)^{-1}X^T.
$$

Its [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md) are $\operatorname{tr}(H_\lambda)$. Thus training error is optimistically biased for independent-copy prediction error by $2\operatorname{tr}(H_\lambda)/n$. The graph exhibits exactly this effect: the dashed training curve keeps falling as $\lambda$ decreases, while the solid test curve eventually rises through [overfitting](../../../../../../overfitting.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
