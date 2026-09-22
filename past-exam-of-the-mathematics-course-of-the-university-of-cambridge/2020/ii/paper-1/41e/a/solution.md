<h1 id="41e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a fixed shift $s$ that is not an [eigenvalue](../../../../../../eigenvalue.md), [inverse iteration](../../../../../../inverse-iteration.md) is the [power method](../../../../../../power-method.md) applied to $(A-sI)^{-1}$. Before normalization, the $k$th vector is proportional to

$$
(A-sI)^{-k}x^{(0)}
=\sum_{i=1}^n c_i(\lambda_i-s)^{-k}w_i.
$$

If $s<\lambda_1$, factor out the first coefficient:

$$
(A-sI)^{-k}x^{(0)}
=c_1(\lambda_1-s)^{-k}
\left[w_1+
\sum_{i=2}^n\frac{c_i}{c_1}
\left(\frac{\lambda_1-s}{\lambda_i-s}\right)^kw_i\right].
$$

Every ratio in parentheses lies strictly between zero and one. The bracket therefore tends to $w_1$, and normalization in the [Euclidean norm](../../../../../../euclidean-norm.md) gives

$$
\boxed{x^{(k)}\longrightarrow\operatorname{sgn}(c_1)w_1.}
$$

This proves the stated convergence to $w_1$ or $-w_1$ and exhibits the [convergence of fixed-shift inverse iteration](../../../../../../convergence-of-fixed-shift-inverse-iteration.md) rate.

Now suppose $\lambda_m<s<\lambda_{m+1}$. The closest eigenvalue to $s$ is one of $\lambda_m$ and $\lambda_{m+1}$.

- If $s-\lambda_m<\lambda_{m+1}-s$, the direction approaches $w_m$, but $(\lambda_m-s)^{-1}<0$, so consecutive iterates alternate signs.
- If $s-\lambda_m>\lambda_{m+1}-s$, the iterates approach one fixed sign of $w_{m+1}$ because $(\lambda_{m+1}-s)^{-1}>0$.
- At the midpoint, the two dominant inverse eigenvalues have equal modulus and opposite signs. Generic iterates alternate between the two normalized combinations proportional to $c_mw_m+c_{m+1}w_{m+1}$ and $-c_mw_m+c_{m+1}w_{m+1}$.

Finally, if $\lambda_n<s$, the closest eigenvalue is $\lambda_n$ and its inverse eigenvalue is negative. Thus the direction approaches the line spanned by $w_n$, while normalized vectors alternate between the two signs. These cases are the [sign behavior of fixed-shift inverse iteration](../../../../../../sign-behavior-of-fixed-shift-inverse-iteration.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [41E](../../41e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
