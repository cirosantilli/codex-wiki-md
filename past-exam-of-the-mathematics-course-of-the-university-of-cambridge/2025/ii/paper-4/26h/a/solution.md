<h1 id="26h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\mu=\mathbb E[X]$ and $\sigma^2=\operatorname{Var}(X)$. Independence of $X$ and the [uniform distribution](../../../../../../continuous-uniform-distribution.md) variable $U$ gives

$$
\mathbb E[Y]=\mathbb E[X]\mathbb E[U]=\boxed{\frac\mu2}.
$$

Also $\mathbb E[U^2]=1/3$, so

$$
\begin{aligned}
\operatorname{Var}(Y)
&=\mathbb E[X^2]\mathbb E[U^2]-\mathbb E[Y]^2\\
&=\frac{\sigma^2+\mu^2}{3}-\frac{\mu^2}{4}.
\end{aligned}
$$

Therefore

$$
\boxed{\operatorname{Var}(Y)=\frac13\operatorname{Var}(X)+\frac1{12}\mathbb E[X]^2}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26H](../../26h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
