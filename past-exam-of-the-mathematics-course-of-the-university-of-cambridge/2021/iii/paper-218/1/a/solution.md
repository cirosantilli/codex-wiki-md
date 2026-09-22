<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $s=x^Tx>0$ and $z=x^TY$. With objective $\lVert Y-x\beta\rVert_2^2+\lambda\beta^2$, [ridge regression](../../../../../../ridge-regression.md) gives

$$
\widehat\beta=\frac z{s+\lambda}.
$$

For the duplicated design, the objective depends on $\beta_1+\beta_2$ through the loss and symmetry makes the minimum-penalty decomposition equal:

$$
\widehat\beta_1=\widehat\beta_2=\frac z{2s+\lambda},
\qquad
\widehat\beta_1+\widehat\beta_2=\frac{2z}{2s+\lambda}.
$$

Duplicating a predictor therefore halves its effective ridge penalty.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
