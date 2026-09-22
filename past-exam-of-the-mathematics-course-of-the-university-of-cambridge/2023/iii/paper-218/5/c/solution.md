<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

When $X^TX=I_p$, expanding the objective separates it by coordinates:

$$
\lVert Y\rVert^2+
\sum_{j=1}^p\{(1+\lambda_2)\beta_j^2
-2(X^TY)_j\beta_j+\lambda_1|\beta_j|\}.
$$

The [soft thresholding](../../../../../../soft-thresholding.md) solution is therefore

$$
\boxed{\widehat\beta_j^E
=\frac{S_{\lambda_1}((X^TY)_j)}{1+\lambda_2},
\qquad j=1,\ldots,p.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
