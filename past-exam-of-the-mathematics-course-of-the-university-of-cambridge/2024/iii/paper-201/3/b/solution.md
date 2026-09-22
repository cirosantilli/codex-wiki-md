<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Each completed visit to radius $r_2$ begins a new radial excursion. By part (a), the conditional probability that the following excursion reaches radius $R$ before radius $r_1$ is

$$
q_R=\frac{\log(r_2/r_1)}{\log(R/r_1)}.
$$

The [Strong Markov property](../../../../../../strong-markov-property.md) at the successive stopping times $\tau_{2k}$ makes these trials independent with the same success probability. Consequently $N(R)$ has a [geometric distribution](../../../../../../geometric-distribution.md) on $\{1,2,\ldots\}$ with parameter $q_R$:

$$
\mathbb P(N(R)>k)=(1-q_R)^k.
$$

As $R\to\infty$, $q_R\to0$ and

$$
q_RN(R)\xrightarrow d\operatorname{Exp}(1),
\qquad
q_R\log R\longrightarrow\log(r_2/r_1).
$$

[Slutsky theorem](../../../../../../slutsky-theorem.md) now gives

$$
\boxed{\frac{N(R)}{\log R}
\xrightarrow d\operatorname{Exp}\!\left(\log(r_2/r_1)\right).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
