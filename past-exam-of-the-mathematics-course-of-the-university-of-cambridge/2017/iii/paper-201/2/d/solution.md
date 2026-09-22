<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $p_m=\mathbb P(S_T=m)$, $p_{m+1}=\mathbb P(S_T=m+1)$, and $q_m=p_m+p_{m+1}$. Part (b) gives

$$
1=2^{-m}(1-q_m)+2^mp_m+2^{m+1}p_{m+1},
$$

so $q_m\leq2^{-m}$. The exit-state decomposition also gives

$$
\frac{\mathbb ES_T}{m}=-1+2q_m+\frac{p_{m+1}}m\longrightarrow-1.
$$

Combining this with part (c), including the upper overshoot, yields

$$
\boxed{\frac{\mathbb ET_m}{m}\longrightarrow\frac74.}
$$

For example, the same calculation supplies the quantitative bound

$$
0\leq\frac74-\frac{\mathbb ET_m}{m}\leq\frac74\left(2+\frac1m\right)2^{-m}.
$$

The asymptotic linear growth is determined by the negative mean increment; the exponentially unlikely upper exit gives a vanishing correction.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
