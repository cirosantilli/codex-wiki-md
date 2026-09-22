<h1 id="30j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each $m$, the displayed objective is the sum of the minimized linear-regression residual sums of squares on the prefix $1{:}m$ and suffix $(m+1){:}n$. Precompute prefix sums of

$$
X_i,quad Y_i,quad X_i^2,quad X_iY_i,quad Y_i^2.
$$

This requires $O(n)$ operations. The corresponding five sums over a suffix are obtained by subtracting a prefix sum from the total.

For any block of $k$ observations, these raw sums give in constant time

$$
S_{xx}=\sum x_i^2-\frac{(\sum x_i)^2}{k},
\quad
S_{xy}=\sum x_iy_i-\frac{(\sum x_i)(\sum y_i)}{k},
\quad
S_{yy}=\sum y_i^2-\frac{(\sum y_i)^2}{k}.
$$

By the formula for the [residual sum of squares in simple linear regression](../../../../../../residual-sum-of-squares-in-simple-linear-regression.md), its minimized loss is

$$
S_{yy}-\frac{S_{xy}^2}{S_{xx}}.
$$

**Hence both losses for a proposed $m$ take constant time. Evaluating their sum for $m=2,\ldots,n-2$ and keeping the minimum is another $O(n)$ scan, so the complete minimization uses $O(n)$ computations.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [30J](../../30j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
