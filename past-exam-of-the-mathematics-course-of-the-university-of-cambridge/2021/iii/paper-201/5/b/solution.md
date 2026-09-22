<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md),

$$
\frac{T_n}{n}\longrightarrow\sigma^2
$$

almost surely. Brownian scaling and a maximal inequality show that changing Brownian time by $o(n)$ changes its value by $o_{\mathbb P}(\sqrt n)$; explicitly, first restrict to $|T_n-n\sigma^2|\leq\delta n$, bound the Brownian maximum over a time interval of length $2\delta n$, and then let $\delta\downarrow0$. Consequently

$$
\frac{B_{T_n}-B_{n\sigma^2}}{\sqrt n}\longrightarrow0
$$

in probability.

But

$$
\frac{B_{n\sigma^2}}{\sqrt n}\sim N(0,\sigma^2)
$$

for every $n$. Since $B_{T_n}$ has the law of $S_n$, [Slutsky theorem](../../../../../../slutsky-theorem.md) proves the [Central limit theorem from the Skorokhod embedding](../../../../../../central-limit-theorem-from-the-skorokhod-embedding.md):

$$
\boxed{\frac{S_n}{\sqrt n}\ \xrightarrow{d}\ N(0,\sigma^2)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
