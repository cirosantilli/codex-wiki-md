<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $q=(\alpha,\beta)^T$, let

$$
A=\begin{pmatrix}100&562.600\\562.600&3331.778\end{pmatrix},
\qquad
\widehat q_0=\binom{1.68782}{0.54218},
$$

and recover the sufficient cross-products from the model1 normal equations by setting $c=A\widehat q_0$ and $s=154.30+\widehat q_0^TA\widehat q_0$. Then

$$
S(q)=s-2q^Tc+q^TAq
$$

is the total squared residual about the fixed line. The squared sum of the ten residuals within each person, summed across people, is

$$
B(q)=100\left(244.1738-2\alpha(47.381)-2\beta(274.898)
+10\alpha^2+2\alpha\beta(56.26)+\beta^2(332.2809)\right).
$$

For one person's ten observations, the marginal covariance matrix is $\tau^2I_{10}+\sigma^2\mathbf1\mathbf1^T$. The [matrix determinant lemma](../../../../../../matrix-determinant-lemma.md) and [Sherman–Morrison formula](../../../../../../sherman-morrison-formula.md) therefore give, up to an additive constant, twice the negative marginal log-likelihood

$$
\omega(\alpha,\beta,\sigma,\tau)
=10\left(9\log\tau^2+\log(\tau^2+10\sigma^2)\right)
+\frac{S(q)}{\tau^2}
-\frac{\sigma^2B(q)}{\tau^2(\tau^2+10\sigma^2)}.
$$

Because the model was fitted with `REML = FALSE`, it minimizes this ordinary marginal maximum-likelihood objective. Thus $(V1,V2,V3,V4)$ belongs to the stated argmin over $alpha,\beta\in\mathbb R$ and $sigma,\tau>0$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
