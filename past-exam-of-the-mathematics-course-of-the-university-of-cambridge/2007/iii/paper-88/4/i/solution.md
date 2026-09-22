<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [octahedral quasirandomness of a three-uniform hypergraph](../../../../../../octahedral-quasirandomness-of-a-three-uniform-hypergraph.md), with its eighth-power normalization. Let $h:X\times Y\times Z\to\{0,1\}$ be the [hypergraph edge](../../../../../../edge-of-a-hypergraph.md) [indicator function](../../../../../../indicator-function.md), define $p=\mathbb E_{x,y,z}h(x,y,z)$, and put $g=h-p$. All [expectations](../../../../../../expected-value.md) are uniform and independent on the indicated [finite sets](../../../../../../finite-set.md). The [hypergraph](../../../../../../hypergraph-split.md) is **$\alpha$-quasirandom** when

$$
\boxed{\|g\|_{\square^3}^8=\mathbb E_{x_0,x_1,y_0,y_1,z_0,z_1}\prod_{i,j,k\in\{0,1\}}g(x_i,y_j,z_k)\leq\alpha.}
$$

The eight triples form the faces of the tripartite octahedral configuration. Repeated choices within a part are included in this normalized average. For real $g$, the expression is nonnegative, since it equals

$$
\mathbb E_{x_0,x_1,y_0,y_1}\left(\mathbb E_z\prod_{i,j\in\{0,1\}}g(x_i,y_j,z)\right)^2.
$$

Thus the condition says that the balanced [hypergraph edge](../../../../../../edge-of-a-hypergraph.md) [indicator function](../../../../../../indicator-function.md) has [three-dimensional box norm](../../../../../../three-dimensional-box-norm.md) at most $\alpha^{1/8}$. If the [norm](../../../../../../norm.md) itself is used as the quasirandomness parameter instead, the eighth-power parameter here is the eighth power of that parameter; stating this convention fixes the quantitative meaning of the counting error.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
