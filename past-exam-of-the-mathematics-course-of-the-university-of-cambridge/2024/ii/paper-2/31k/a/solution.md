<h1 id="31k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start with the root region $\mathbb R^p$. For any current terminal region $R$, coordinate $k$, and threshold $s$, form

$$
R_-=\{x\in R:x_k\leq s\},\qquad
R_+=\{x\in R:x_k>s\},
$$

discarding splits that leave an empty child. For each child use its training-response mean

$$
\widehat\gamma_\pm=
\frac{\sum_iY_i'\mathbf1_{R_\pm}(X_i')}
{\sum_i\mathbf1_{R_\pm}(X_i')}.
$$

Compare candidate splits by the resulting residual sum of squares

$$
\sum_{X_i'\in R_-}(Y_i'-\widehat\gamma_-)^2+
\sum_{X_i'\in R_+}(Y_i'-\widehat\gamma_+)^2,
$$

together with the unchanged residual sums in the other leaves. Choose the leaf, coordinate, and threshold minimizing the total. Replace that leaf by its two children and repeat until the stopping rule or the prescribed $J$ leaves is reached. The resulting terminal regions are $\widehat R_1,\ldots,\widehat R_J$, and

$$
\widehat\gamma_j=
\frac{\sum_iY_i'\mathbf1_{\widehat R_j}(X_i')}
{\sum_i\mathbf1_{\widehat R_j}(X_i')}.
$$

This is the standard [regression tree](../../../../../../regression-tree.md) construction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31K](../../31k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
