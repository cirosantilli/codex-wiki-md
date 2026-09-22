<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $p>1$, the bound $X_k\leq2$ ensures the finite [moment](../../../../../moment.md) $m_p=\mathbb EX_1^p\leq2^p$. By [Jensen's inequality](../../../../../jensen-s-inequality.md), $m_p\geq(\mathbb EX_1)^p=1$. The process $Z_k=Y_k^p$ is an [adapted](../../../../../adapted-process.md), nonnegative [integrable random variable](../../../../../integrable-random-variable.md) at each time, and [independence](../../../../../independent-random-variables.md) gives

$$
\mathbb E[Z_{k+1}\mid\mathcal H_k]
=Y_k^p\mathbb EX_{k+1}^p=m_pZ_k\geq Z_k.
$$

Thus $(Z_k)$ is a [submartingale](../../../../../submartingale.md), and $\mathbb EZ_n=m_p^n$. The [Doob maximal inequality for a nonnegative submartingale](../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) states that $c\mathbb P(\max_{k\leq n}Z_k\geq c)\leq\mathbb EZ_n$ for $c>0$. Apply it with $c=\lambda^p$. Since the power [function](../../../../../function-split.md) is increasing on $[0,\infty)$,

$$
\mathbb P\left(\max_{1\leq k\leq n}Y_k\geq\lambda\right)
\leq\frac{m_p^n}{\lambda^p}.
$$

Combining this with the preceding bound gives

$$
\boxed{\mathbb P\left(\max_{1\leq k\leq n}Y_k\geq\lambda\right)
\leq\min\left\{\lambda^{-1},\ m_p^n\lambda^{-p}\right\}.}
$$

The result is a bound on the running maximum, which is why a maximal [inequality](../../../../../inequality-mathematics.md) for a [submartingale](../../../../../submartingale.md), rather than an estimate of the single terminal [random variable](../../../../../random-variable-split.md), is needed.[§4.4, Theorem 4.4.2, printed p. 235: the submartingale maximal inequality](../../../../../probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
