<h1 id="30l/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The hypothesis class and margin loss are

$$
\boxed{\mathcal H
=\{h_M:x\mapsto x^TMx,\ M\succeq0,\ \operatorname{Tr}M\leq s\}}
$$

and

$$
\boxed{\phi(u)=\log(1+e^{-u})}.
$$

Thus this is a [positive semidefinite quadratic-form classifier](../../../../../../positive-semidefinite-quadratic-form-classifier.md) with [logistic loss](../../../../../../logistic-loss.md). Its empirical risk, viewed as a function of the matrix parameter, is

$$
F(M)=\widehat R_\phi(h_M)
=\frac1n\sum_{j=1}^n
\log\left(1+\exp(-Y_jX_j^TMX_j)\right).
$$

Differentiating under the sum shows that

$$
\nabla F(M)
=-\frac1n\sum_{j=1}^n
Y_jX_jX_j^T
\frac{\exp(-Y_jX_j^TMX_j)}
{1+\exp(-Y_jX_j^TMX_j)}.
$$

Hence the displayed $g_i$ is exactly $\nabla F(M^{(i)})$, and the algorithm is [projected gradient descent](../../../../../../projected-gradient-descent.md) on the [positive semidefinite trace ball](../../../../../../positive-semidefinite-trace-ball.md).

The scalar factor multiplying each $Y_jX_jX_j^T$ lies in $[0,1]$. Since

$$
\|xx^T\|_F
=\sqrt{\operatorname{Tr}(xx^Txx^T)}
=\|x\|_2^2,
$$

we have the uniform gradient bound

$$
\|g_i\|_F\leq\frac1n\sum_{j=1}^n\|X_j\|_2^2
\leq C^2.
$$

Let $\widehat M$ parametrize the empirical minimizer $\widehat h$. Positive semidefiniteness gives

$$
\|\widehat M\|_F
=\left(\sum_r\lambda_r(\widehat M)^2\right)^{1/2}
\leq\sum_r\lambda_r(\widehat M)
=\operatorname{Tr}\widehat M
\leq s.
$$

Thus the initial distance from $M^{(1)}=0$ to $\widehat M$ is at most $D=s$, while the gradient bound is $G=C^2$.

The [averaged projected-gradient bound](../../../../../../averaged-projected-gradient-bound.md), in its slightly looser form

$$
F(\bar M)-F(\widehat M)
\leq\frac{D^2}{\eta k}+\eta G^2,
$$

applies because $F$ is convex. Choose

$$
\boxed{\eta=\frac{s}{C^2\sqrt k}}.
$$

Substitution gives

$$
\widehat R_\phi(\bar h)-\widehat R_\phi(\widehat h)
=F(\bar M)-F(\widehat M)
\leq\frac{s^2}{\eta k}+\eta C^4
=\boxed{\frac{2sC^2}{\sqrt k}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30L](../../30l.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
