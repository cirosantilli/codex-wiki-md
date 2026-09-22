<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First prove the [pair-factor correlation bound for the three-dimensional box norm](../../../../../../pair-factor-correlation-bound-for-the-three-dimensional-box-norm.md). For real $g$ and three [functions](../../../../../../function-split.md) $a(y,z),b(x,z),c(x,y)$ bounded in absolute value by one, let

$$
T=\mathbb E_{x,y,z}g(x,y,z)a(y,z)b(x,z)c(x,y).
$$

Apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) in $(y,z)$, placing the $x$ average inside and removing $a$. This gives

$$
|T|^2\leq\mathbb E_{y,z}\left|\mathbb E_xg(x,y,z)b(x,z)c(x,y)\right|^2.
$$

Expand this square, with independent $x_0,x_1$. Apply Cauchy-Schwarz in $(x_0,x_1,z)$, removing the product $b(x_0,z)b(x_1,z)$. The result is

$$
|T|^4\leq\mathbb E_{x_0,x_1,z}\left|\mathbb E_y g(x_0,y,z)g(x_1,y,z)c(x_0,y)c(x_1,y)\right|^2.
$$

Expand with independent $y_0,y_1$ and apply Cauchy-Schwarz in $(x_0,x_1,y_0,y_1)$, removing the four $c$ factors. Then

$$
|T|^8\leq\mathbb E_{x_0,x_1,y_0,y_1}\left|\mathbb E_z\prod_{i,j\in\{0,1\}}g(x_i,y_j,z)\right|^2=\|g\|_{\square^3}^8.
$$

Therefore **$|T|\leq\|g\|_{\square^3}$**, with no independence assumption on the three pair [functions](../../../../../../function-split.md).

In this [multipartite hypergraph](../../../../../../multipartite-hypergraph.md), a simplex is a [three-uniform tetrahedron](../../../../../../three-uniform-tetrahedron.md): one [vertex of a hypergraph](../../../../../../vertex-of-a-hypergraph.md) from each of $X,Y,Z,W$, with all four possible triples present. Write the corresponding [hypergraph edge](../../../../../../edge-of-a-hypergraph.md) [indicator functions](../../../../../../indicator-function.md) as $h_1(x,y,z),h_2(x,y,w),h_3(x,z,w),h_4(y,z,w)$, of [subset densities](../../../../../../density-of-a-finite-subset.md) $p,q,r,s$. Its normalized count is

$$
t=\mathbb E_{x,y,z,w}h_1h_2h_3h_4.
$$

Telescope the product exactly:

$$
h_1h_2h_3h_4-pqrs=(h_1-p)h_2h_3h_4+p(h_2-q)h_3h_4+pq(h_3-r)h_4+pqr(h_4-s).
$$

For the first term fix $w$. The remaining three factors are bounded pair [functions](../../../../../../function-split.md) of $(x,y)$, $(x,z)$ and $(y,z)$, so the inequality just proved bounds its $(x,y,z)$ average by $\|h_1-p\|_{\square^3}\leq\alpha^{1/8}$. Averaging over $w$ preserves that bound. For each other term fix the [vertex of a hypergraph](../../../../../../vertex-of-a-hypergraph.md) outside its balanced triple and apply the same argument, allowing an unused pair factor to be identically one. The [subset density](../../../../../../density-of-a-finite-subset.md) prefactors are at most one. Hence

$$
\boxed{|t-pqrs|\leq4\alpha^{1/8}.}
$$

Multiplying by $|X||Y||Z||W|$ gives

$$
\boxed{|\#\text{simplices}-pqrs|X||Y||Z||W||\leq4\alpha^{1/8}|X||Y||Z||W|.}
$$

Thus one may take the absolute constant $C=4$. This proves the complete-pair-support case of the [tetrahedron counting lemma](../../../../../../tetrahedron-counting-lemma.md) directly; no lower bound on $p,q,r,s$ is needed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
