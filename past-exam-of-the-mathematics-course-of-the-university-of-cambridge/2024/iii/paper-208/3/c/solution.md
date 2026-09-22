<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\varepsilon_1,\ldots,\varepsilon_n$ be independent $\operatorname{Bernoulli}(\lambda/n)$ variables and $S_n=\sum_i\varepsilon_i$. Apply the [tensorization of entropy](../../../../../../tensorization-of-entropy.md) to $f(S_n)$ and then apply the stated Bernoulli log-Sobolev inequality in each coordinate. If $S_n^{(i)}=S_n-\varepsilon_i$, this gives

$$
\operatorname{Ent}(f(S_n))
\leq n\frac{\lambda}{n}\left(1-\frac{\lambda}{n}\right)
\mathbb E\left[
\frac{|Df(S_n^{(i)})|^2}{f(S_n)}\right].
$$

For each fixed $i$, $(S_n^{(i)},\varepsilon_i)$ converges in distribution to $(X,0)$, where $X\sim\operatorname{Poisson}(\lambda)$. The [Poisson limit theorem](../../../../../../poisson-limit-theorem.md) in fact gives convergence in total variation. The assumptions $K_1\leq f\leq K_2$ and $|Df|\leq K_3$ make all displayed integrands bounded, so expectations and entropy pass to the limit. Since $n(\lambda/n)(1-\lambda/n)\to\lambda$,

$$
\boxed{\operatorname{Ent}(f(X))
\leq\lambda\mathbb E\left[\frac{|Df(X)|^2}{f(X)}\right].}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
