<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

If $X_0\sim N(0,(2\lambda)^{-1})$ independently of $B$, then

$$
\operatorname{Var}(X_t)
=e^{-2\lambda t}\frac1{2\lambda}
+\frac{1-e^{-2\lambda t}}{2\lambda}
=\frac1{2\lambda}.
$$

Thus $X_t\sim N(0,(2\lambda)^{-1})$ for every $t$. For $0<s<t$, the Markov decomposition

$$
X_t=e^{-\lambda(t-s)}X_s
+\int_s^te^{-\lambda(t-r)}\,dB_r
$$

has an increment independent of $X_s$, and hence

$$
\operatorname{Cov}(X_t,X_s)
=\frac{e^{-\lambda(t-s)}}{2\lambda}.
$$

This is the stationary Ornstein-Uhlenbeck covariance.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
