<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With the normalization used here, the [Lasso](../../../../../../lasso.md) estimator minimizes

$$
\frac1{2n}\lVert Y-X\beta\rVert_2^2+\lambda\lVert\beta\rVert_1.
$$

Optimality at $\widehat\beta$ relative to the feasible point $\beta^0$ gives

$$
\frac1{2n}\lVert Y-X\widehat\beta\rVert_2^2+\lambda\lVert\widehat\beta\rVert_1
\leq\frac1{2n}\lVert Y-X\beta^0\rVert_2^2+\lambda\lVert\beta^0\rVert_1.
$$

The columns of $X$ are centered, so $X^T\mathbf1=0$ and the centered noise produces the same [score function](../../../../../../informant-function.md) as $\varepsilon$. Expanding the two squared norms and cancelling the noise norm yields the standard [Basic inequality for the Lasso](../../../../../../basic-inequality-for-the-lasso.md)

$$
\frac1{2n}\lVert X(\widehat\beta-\beta^0)\rVert_2^2
\leq\frac1n(\widehat\beta-\beta^0)^TX^T\varepsilon
+\lambda\lVert\beta^0\rVert_1-\lambda\lVert\widehat\beta\rVert_1.
$$

Thus the displayed inequality in the question has a factor-of-two typo: its left side should be $\lVert X(\widehat\beta-\beta^0)\rVert_2^2/(2n)$, or both terms on its right should be doubled. No scaling of the usual squared-error Lasso objective produces the three displayed coefficients simultaneously. Parts b and d explicitly ask us to use the stated inequality, so their requested constants follow from that stated version.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
