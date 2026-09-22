<h1 id="26h/solution">Solution</h1>

↑ **Parent:** [26H](../26h.md)

If the variables are [independent random variables](../../../../../independent-random-variables.md), apply the defining product rule first to indicator functions, then to simple functions, and finally use bounded measurable approximation to obtain the displayed identity. Conversely, choosing $f_n=1_{A_n}$ gives

$$
\mathbb P(X_1\in A_1,\ldots,X_N\in A_N)=\prod_n\mathbb P(X_n\in A_n),
$$

which is independence.

Let $S_m=\sum_{n\leq m}X_n$. Independence and zero means imply orthogonality in $L^2$, so

$$
\|S_m-S_l\|_2^2=\sum_{n=l+1}^mσ_n^2.
$$

If the variance series converges, $(S_m)$ is Cauchy in the complete space $L^2$ and hence converges there. Conversely, $L^2$ convergence makes $(S_m)$ Cauchy, so every tail of the nonnegative variance series tends to zero; therefore $\sum_nσ_n^2<∞$.

## ↑ Ancestors (10)

1. [26H](../26h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
