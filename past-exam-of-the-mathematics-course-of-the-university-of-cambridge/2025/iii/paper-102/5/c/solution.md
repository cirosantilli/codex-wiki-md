<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [dominance order](../../../../../../dominance-order.md) is

$$
\mu\preceq\lambda
\quad\Longleftrightarrow\quad
\lambda-\mu=\sum_i n_i\alpha_i
\quad(n_i\in\mathbb Z_{\geq0}).
$$

Suppose $\lambda\ne\mu$. Put $\delta=\lambda-\mu$. Since $\mu$ is dominant,

$$
(\lambda,\delta)=(\mu,\delta)+(\delta,\delta)>0.
$$

Writing $\delta=\sum_i n_i\alpha_i$, some index with $n_i>0$ therefore satisfies $(\lambda,\alpha_i)>0$, equivalently $\langle\lambda,\alpha_i^\vee\rangle>0$. The $\mathfrak{sl}_2$ lowering operator

$$
f_i:V_\lambda\longrightarrow V_{\lambda-\alpha_i}
$$

is injective by the [Injectivity of sl2 lowering above weight zero](../../../../../../injectivity-of-sl2-lowering-above-weight-zero.md). Hence

$$
\operatorname{mult}(\lambda)
\leq\operatorname{mult}(\lambda-\alpha_i).
$$

The new weight still dominates $\mu$ in the partial order. Iterating until reaching $\mu$ gives

$$
\boxed{\operatorname{mult}(\mu)\geq\operatorname{mult}(\lambda)}.
$$

This is the [weight multiplicity decreases away from a dominant weight](../../../../../../weight-multiplicity-decreases-away-from-a-dominant-weight.md) property.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
