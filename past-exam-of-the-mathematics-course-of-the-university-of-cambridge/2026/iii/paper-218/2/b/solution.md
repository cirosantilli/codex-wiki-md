<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conditional on $X_1,\ldots,X_n$, the $L$ selected class indicators are independent Bernoulli variables. Therefore

$$
e_1(x)=\frac1L\sum_{\ell=1}^Lp_1(X_{(\ell)})
$$

and

$$
\mathbb E\left[(\widehat p_1(x)-e_1(x))^2\mid X_1,\ldots,X_n\right]
=\frac1{L^2}\sum_{\ell=1}^Lp_1(X_{(\ell)})(1-p_1(X_{(\ell)}))
\leq\frac1{4L}\leq\frac1L.
$$

Taking expectations proves the claim.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
