<h1 id="30k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\Delta M_n=M_n-M_{n-1}$. Conditional on $\mathcal F_{n-1}$, the variables $X_{n-1}$, $M_{n-1}$, and $A_n$ are known, while $\mathbb E[\Delta M_n\mid\mathcal F_{n-1}]=0$. Hence

$$
\begin{aligned}
\operatorname{Cov}(X_n,M_n\mid\mathcal F_{n-1})
&=\operatorname{Cov}(A_n\Delta M_n,\Delta M_n\mid\mathcal F_{n-1})\\
&=A_n\operatorname{Var}(\Delta M_n\mid\mathcal F_{n-1})\\
&=A_n\operatorname{Var}(M_n\mid\mathcal F_{n-1}).
\end{aligned}
$$

The denominator is positive almost surely, so the [recovery of a martingale-transform integrand by conditional covariance](../../../../../../recovery-of-a-martingale-transform-integrand-by-conditional-covariance.md) gives

$$
\boxed{A_n=
\frac{\operatorname{Cov}(X_n,M_n\mid\mathcal F_{n-1})}
{\operatorname{Var}(M_n\mid\mathcal F_{n-1})}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30K](../../30k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
