<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) says that for a linear map $T:V\to W$ with finite-dimensional domain, $\dim V=\dim\ker T+\dim\operatorname{im}T$. Apply it to $\beta|_{\operatorname{im}\alpha}$. Its image is $\operatorname{im}(\beta\alpha)$ and its kernel is $\operatorname{im}\alpha\cap\ker\beta$, so

$$
\boxed{\dim\operatorname{im}\alpha
=\dim\operatorname{im}(\beta\alpha)
+\dim(\operatorname{im}\alpha\cap\ker\beta).}
$$

Since $\operatorname{im}(\alpha\gamma)\subseteq\operatorname{im}\alpha$,

$$
\dim(\operatorname{im}(\alpha\gamma)\cap\ker\beta)
\leq\dim(\operatorname{im}\alpha\cap\ker\beta).
$$

Using the preceding identity for both restrictions and rearranging gives

$$
\boxed{\dim\operatorname{im}(\beta\alpha)+\dim\operatorname{im}(\alpha\gamma)
\leq\dim\operatorname{im}\alpha+\dim\operatorname{im}(\beta\alpha\gamma).}
$$

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
