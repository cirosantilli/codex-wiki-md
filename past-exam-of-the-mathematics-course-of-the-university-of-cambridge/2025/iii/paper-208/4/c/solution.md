<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each $i$, the [total variation distance](../../../../../../total-variation-distance.md) between $\operatorname{Bernoulli}(p_i)$ and $\operatorname{Poisson}(p_i)$ is

$$
p_i(1-e^{-p_i})\leq p_i^2.
$$

Indeed, compare their masses at zero, one, and the Poisson tail; the positive excess of Bernoulli mass at one is $p_i(1-e^{-p_i})$. A maximal coupling therefore gives a pair $(X_i,N_i)$ with mismatch probability at most $p_i^2$. Couple these pairs independently. Then

$$
\mathbb P\left(\sum_iX_i\ne\sum_iN_i\right)
\leq\sum_i p_i^2
$$

by the union bound. Since $\sum_iN_i\sim\operatorname{Poisson}(\sum_ip_i)=\operatorname{Poisson}(\nu)$, part (b) yields

$$
\boxed{d_{\mathrm{TV}}(P,Q)\leq\sum_{i=1}^np_i^2.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
