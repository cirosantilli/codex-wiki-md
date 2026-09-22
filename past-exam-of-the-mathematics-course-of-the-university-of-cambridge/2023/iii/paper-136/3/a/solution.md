<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $G=\operatorname{Gal}(L/K)$. The lower [ramification groups](../../../../../../ramification-group.md) are $G_{-1}=G$ and, for $i\geq0$,

$$
G_i=\{\sigma\in G:v_L(\sigma(x)-x)\geq i+1
\text{ for every }x\in\mathcal O_L\}.
$$

If $L/K$ is totally ramified and $\pi_L$ is a [uniformizer](../../../../../../uniformizer.md), then $\mathcal O_L=\mathcal O_K[\pi_L]$. Factoring $F(\sigma\pi_L)-F(\pi_L)$ by $\sigma\pi_L-\pi_L$ for $F\in\mathcal O_K[X]$ proves the [uniformizer criterion for lower ramification groups](../../../../../../uniformizer-criterion-for-lower-ramification-groups.md)

$$
G_i=\{\sigma\in G:v_L(\sigma(\pi_L)-\pi_L)\geq i+1\}.
$$

For $\sigma\in G_0$, define

$$
\theta(\sigma)=\overline{\frac{\sigma(\pi_L)}{\pi_L}}\in k_L^\times.
$$

The [inertia group](../../../../../../inertia-group.md) $G_0$ acts trivially on $k_L$, so $\theta(\sigma\tau)=\theta(\sigma)\theta(\tau)$. Its kernel consists exactly of those $\sigma$ for which $\sigma(\pi_L)/\pi_L\equiv1$ modulo the maximal ideal, namely $G_1$. The [first isomorphism theorem](../../../../../../first-isomorphism-theorem.md) therefore gives an injection

$$
\boxed{G_0/G_1\hookrightarrow k_L^\times.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
