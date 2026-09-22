<h1 id="22f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [continuous dual space](../../../../../../continuous-dual-space-split.md) of a normed vector space $V$ is

$$
V^*=\{f:V\to\mathbb F:f\text{ is linear and continuous}\},
$$

with the [operator norm](../../../../../../operator-norm.md)

$$
\lVert f\rVert=\sup_{\lVert v\rVert\leq1}|f(v)|.
$$

Let $(f_n)$ be a [Cauchy sequence](../../../../../../cauchy-sequence.md) in this norm. For each $v\in V$,

$$
|f_n(v)-f_m(v)|\leq\lVert f_n-f_m\rVert\,\lVert v\rVert,
$$

so $(f_n(v))$ is Cauchy in the scalar field. Define $f(v)=\lim_n f_n(v)$. Passing to limits in the linearity identities shows that $f$ is linear.

A norm-Cauchy sequence is bounded, say $\lVert f_n\rVert\leq M$. Hence $|f(v)|\leq M\lVert v\rVert$, so $f\in V^*$. Given $\varepsilon>0$, choose $N$ such that $\lVert f_n-f_m\rVert<\varepsilon$ for $m,n\geq N$. Letting $m\to\infty$ gives

$$
|f_n(v)-f(v)|\leq\varepsilon\lVert v\rVert
$$

for every $v$, and therefore $\lVert f_n-f\rVert\leq\varepsilon$. Thus $f_n\to f$ in operator norm, proving [completeness of the dual space](../../../../../../completeness-of-the-dual-space.md): $V^*$ is Banach.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22F](../../22f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
