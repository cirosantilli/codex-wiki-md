<h1 id="29l/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $v=\sigma^2$. For one observation, the score is

$$
s_\mu(x;\mu,v)=\frac{x-\mu}{v},
\qquad
s_v(x;\mu,v)=-\frac1{2v}+\frac{(x-\mu)^2}{2v^2},
$$

and

$$
I_1(\mu,v)=
\begin{pmatrix}v^{-1}&0\\0&(2v^2)^{-1}\end{pmatrix}.
$$

Under the restriction $v=1$, the [restricted maximum-likelihood estimator](../../../../../../../restricted-maximum-likelihood-estimator.md) is $\widetilde\mu=\bar X$. At $(\bar X,1)$ the first score component is zero, while the second is

$$
\frac12\sum_{i=1}^n\bigl((X_i-\bar X)^2-1\bigr).
$$

Since $I_1(\bar X,1)^{-1}=\operatorname{diag}(1,2)$, substitution into the score statistic gives

$$
\boxed{
T_n=\left[\frac1{\sqrt{2n}}
\sum_{i=1}^n\bigl((X_i-\bar X)^2-1\bigr)\right]^2.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [29L](../../../29l.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
