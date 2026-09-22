<h1 id="25k/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A necessary qualification is $\sigma^2>0$. As printed, the assumptions also permit $X_i=0$ almost surely; then $\mathbb P(A_n)=0$ for every $K>0$, so the asserted positive lower bound is false. Assume the intended nondegenerate case.

The [central limit theorem](../../../../../../central-limit-theorem.md) states that independent identically distributed variables with mean zero and finite positive variance satisfy $S_n/(\sigma\sqrt n)\Rightarrow Z$, where $Z\sim N(0,1)$. Since the [normal distribution](../../../../../../normal-distribution.md) has no atom at $K/\sigma$,

$$
\mathbb P(A_n)\longrightarrow\mathbb P(Z\geq K/\sigma)=1-\Phi(K/\sigma)>0.
$$

For example,

$$
\boxed{c=\tfrac12[1-\Phi(K/\sigma)]\text{ works for all sufficiently large }n.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [25K](../../25k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
