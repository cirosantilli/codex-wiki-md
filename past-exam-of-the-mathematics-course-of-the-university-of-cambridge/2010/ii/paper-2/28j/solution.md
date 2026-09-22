<h1 id="28j/solution">Solution</h1>

↑ **Parent:** [28J](../28j.md)

Let $F_n(x)=n^{-1}\sum_i\mathbf1_{\{X_i\leq x\}}$. The [Kolmogorov-Smirnov statistic](../../../../../kolmogorov-smirnov-statistic.md) is $D_n=\sup_x|F_n(x)-F(x)|$, often reported as $\sqrt nD_n$. Under the simple null, the [probability integral transform](../../../../../probability-integral-transform.md) makes $U_i=F(X_i)$ independent uniform variables on $[0,1]$. Strict monotonicity and continuity identify the empirical distribution under this change of coordinates, so

$$
D_n=\sup_{0\leq u\leq1}|G_n(u)-u|.
$$

Its null law is therefore independent of $F$.

For the composite null, the joint density is $\theta^{-n}\prod_i\mathbf1_{\{0\leq x_i\leq\theta\}}$. Its parameter dependence is only through $M=\max_iX_i$, proving sufficiency by the [Fisher-Neyman factorization theorem](../../../../../fisher-neyman-factorization-theorem.md); the larger statistic $(J,M)$ is sufficient too. Ties have probability zero. For fixed $j$, the density of $(J=j,M=\xi)$ is $\xi^{n-1}/\theta^n$, $0<\xi<\theta$, because the other coordinates range independently over $[0,\xi]$. Dividing the joint density by this marginal gives conditional density

$$
\xi^{-(n-1)}\prod_{i\ne j}\mathbf1_{\{0\leq x_i\leq\xi\}}.
$$

Thus the remaining observations are conditionally independent $U[0,\xi]$.

For $n\geq2$, discard the maximum and apply the [Kolmogorov-Smirnov test](../../../../../kolmogorov-smirnov-test.md) to the $n-1$ ratios $X_i/M$, $i\ne J$, against $U[0,1]$. **Use the ordinary null critical values for sample size $n-1$.** Its conditional, hence unconditional, level is independent of $\theta$. Keeping the fitted maximum and using the ordinary $n$-sample critical values would not have that justification.

## ↑ Ancestors (10)

1. [28J](../28j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
