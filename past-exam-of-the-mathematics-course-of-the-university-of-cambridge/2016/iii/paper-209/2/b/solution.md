<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For real $v$, $\overline{\varphi(v)}=\varphi(-v)$. Expand the [complex covariance](../../../../../../complex-covariance.md) of the sample averages. Terms indexed by distinct observations vanish because the observations are [independent](../../../../../../independent-random-variables.md); each diagonal term equals $\mathbb E e^{i(u-v)X_1}-\varphi(u)\overline{\varphi(v)}$. Hence

$$
\boxed{\operatorname{Cov}_{\mathbb C}\bigl(\varphi_n(u),\varphi_n(v)\bigr)
=\frac1n\bigl(\varphi(u-v)-\varphi(u)\varphi(-v)\bigr).}
$$

Taking $v=u$ and using $\varphi(0)=1$ gives the exact [variance](../../../../../../variance-split.md):

$$
\boxed{\operatorname{Var}_{\mathbb C}(\varphi_n(u))
=\frac{1-|\varphi(u)|^2}{n}\leq\frac1n.}
$$

The upper bound follows from $|\varphi(u)|\leq\mathbb E|e^{iuX_1}|=1$, and holds without any moment assumptions on $X_1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
