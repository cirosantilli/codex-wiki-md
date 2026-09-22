<h1 id="18h/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For arbitrary $\beta$,

$$
\mathbb E\|\widehat\beta\|^2
=\|\beta\|^2
+\operatorname{tr}\!\left(\sigma^2(X^TX)^{-1}\right)
=\|\beta\|^2+\sigma^2\sum_{j=1}^p\lambda_j^{-1}.
$$

Independence from part (ii) and $Z=n\widehat\sigma^2/\sigma^2\sim\chi^2_{n-p}$ give

$$
\mathbb ET
=\frac{\mathbb E\|\widehat\beta\|^2}{\sigma^2}
\mathbb E\!\left(\frac1Z\right).
$$

Because $n-p>2$,

$$
\mathbb E(Z^{-1})=\frac1{n-p-2}.
$$

Thus

$$
\boxed{
\mathbb ET
=\frac{\|\beta\|^2/\sigma^2
+\sum_{j=1}^p\lambda_j^{-1}}
{n-p-2}
}.
$$

## ↑ Ancestors (11)

1. [V](../v.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
