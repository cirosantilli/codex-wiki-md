<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For Borel sets $A_1,\ldots,A_n$, multiply the finite-time [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) into the product law of the increments:

$$
\begin{aligned}
\mathbb P_n^\lambda(X_1\in A_1,\ldots,X_n\in A_n)
&=\mathbb E\left[\prod_{j=1}^n\frac{e^{\lambda X_j}}{\phi(\lambda)}\mathbf1_{\{X_j\in A_j\}}\right]\\
&=\prod_{j=1}^n\int_{A_j}\frac{e^{\lambda x}}{\phi(\lambda)}\,\mu(dx).
\end{aligned}
$$

The factorization, extended from rectangles to the product [sigma-algebra](../../../../../../sigma-algebra.md), proves [independence](../../../../../../independent-random-variables.md) and identical distributions. Their common law is the [exponential tilting](../../../../../../exponential-tilting.md)

$$
\boxed{\mu^\lambda(dx)=\frac{e^{\lambda x}}{\phi(\lambda)}\mu(dx).}
$$

For $\lambda>0$, $|x|e^{\lambda x}$ is bounded on $x\leq0$, while $xe^{\lambda x}\leq C_\varepsilon e^{(\lambda+\varepsilon)x}$ on $x\geq0$. Choosing a small two-sided neighborhood of $\lambda$ still contained in $(0,\infty)$ gives an integrable dominating function for the derivative. [Differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) then yields

$$
\phi'(\lambda)=\int xe^{\lambda x}\,\mu(dx),\qquad
\boxed{\mathbb E^\lambda X_1=\frac{\phi'(\lambda)}{\phi(\lambda)}\quad(\lambda>0).}
$$

The [mean under one-sided exponential tilting](../../../../../../mean-under-one-sided-exponential-tilting.md) needs an endpoint qualification. At $\lambda=0$, finiteness of positive [exponential moments](../../../../../../exponential-moment.md) makes $X_1^+$ integrable, but gives no integrability of $X_1^-$. The formula holds with the right derivative and the extended mean $\phi'_+(0)=\mathbb EX_1\in[-\infty,\infty)$. To see this, apply [monotone convergence](../../../../../../monotone-convergence-theorem.md) to $(1-e^{-hX_1^-})/h$ and [dominated convergence](../../../../../../dominated-convergence-theorem.md) to $(e^{hX_1^+}-1)/h$ as $h\downarrow0$. A finite mean at zero is not guaranteed by the printed hypotheses: $\mu(\{-j\})=6/(\pi^2j^2)$, $j\geq1$, has finite $\phi(\lambda)$ for every $\lambda\geq0$ but $\mathbb EX_1=-\infty$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
