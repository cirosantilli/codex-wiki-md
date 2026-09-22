<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Writing $X_1=\mu+Z$ with $Z\sim N(0,1)$ gives

$$
\mathbb E S=\mathbb E X_1^2-1=\mu^2,
$$

so $S$ is unbiased. Its mean square error is therefore its variance. Since

$$
\mathbb E X_1^4
=\mathbb E(\mu+Z)^4
=\mu^4+6\mu^2+3,
$$

we obtain

$$
\operatorname{MSE}(S)
=\operatorname{var}(X_1^2)
=\mu^4+6\mu^2+3-(\mu^2+1)^2
=\boxed{4\mu^2+2}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
