<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [coarse embedding](../../../../../coarse-embedding.md) $f:X\to Y$ has nondecreasing control functions $\rho_-,\rho_+$ such that

$$
\rho_-(d_X(x,y))\leq d_Y(f(x),f(y))\leq\rho_+(d_X(x,y)),
\qquad \rho_-(t)\longrightarrow\infty.
$$

A family is a [uniform coarse embedding of a family of metric spaces](../../../../../uniform-coarse-embedding-of-a-family-of-metric-spaces.md) when all its maps use the same controls.

For $H_n=\{0,1\}^n$ with the [Hamming distance](../../../../../hamming-distance.md), the coordinate map into $\ell_1^n$ satisfies

$$
\|x-y\|_1=d_H(x,y),
$$

so the cubes embed isometrically and uniformly into $L^1$. The same coordinate map into $\ell_2^n$ satisfies

$$
\|x-y\|_2=\sqrt{d_H(x,y)}.
$$

Thus they also uniformly coarsely embed into $L^2$, with $\rho_-(t)=\rho_+(t)=\sqrt t$. This is the [Hamming cube as an L1 and L2 metric](../../../../../hamming-cube-as-an-l1-and-l2-metric.md).

For a finite graph $G=(V,E)$, define

$$
h(G)=\min_{0<|S|\leq|V|/2}\frac{|\partial_ES|}{|S|}.
$$

An [expander family](../../../../../expander-graph.md) is a sequence of graphs with orders tending to infinity, uniformly bounded degrees, and $h(G)$ uniformly bounded below.

Now let $|V|=n$ and let $M$ be a median of $f:V\to\mathbb R$. Put

$$
g=(f-M)_+,
\qquad k=(M-f)_+.
$$

Both supports have at most $n/2$ vertices. The [layer cake representation](../../../../../layer-cake-representation.md) and the definition of $h$ give

$$
\begin{aligned}
\sum_{x,y}a_{xy}|g(x)-g(y)|
&=2\int_0^\infty|\partial_E\{g>t\}|\,dt\\
&\geq2h\int_0^\infty|\{g>t\}|\,dt
=2h\sum_xg(x),
\end{aligned}
$$

and the same holds for $k$. Since their supports are disjoint,

$$
|f(x)-f(y)|=|g(x)-g(y)|+|k(x)-k(y)|.
$$

Adding gives

$$
\boxed{\sum_{x,y}a_{xy}|f(x)-f(y)|
\geq2h\sum_x|f(x)-M|}.
$$

The [triangle inequality](../../../../../triangle-inequality.md) also gives

$$
\sum_{x,y}|f(x)-f(y)|
\leq2n\sum_x|f(x)-M|,
$$

and hence

$$
\boxed{\sum_{x,y}a_{xy}|f(x)-f(y)|
\geq\frac hn\sum_{x,y}|f(x)-f(y)|}.
$$

Represent an $L^1$-valued map as scalar functions on the underlying measure space and integrate this inequality. The result is the [L1 Poincare inequality for an expander graph](../../../../../l1-poincare-inequality-for-an-expander-graph.md).

Suppose next that $G$ is $d$-regular and $F:V\to L^1$ is noncontracting with Lipschitz constant $D$. The Poincare inequality gives

$$
ndD\geq\sum_{x,y}a_{xy}\|F(x)-F(y)\|_1
\geq\frac hn\sum_{x,y}d_G(x,y).
$$

A ball of radius $r$ in a graph of maximum degree $d$ has at most

$$
1+d\sum_{j=0}^{r-1}(d-1)^j\leq e d^r
$$

vertices. Therefore, for

$$
0\leq r\leq\frac{\log(n/2)-1}{\log d},
$$

at least $n/2$ vertices lie outside the radius-$r$ ball about each vertex. Integrating the tail count of the distance gives

$$
\sum_{x,y}d_G(x,y)
\geq\frac{n^2}{2}\frac{\log(n/2)-1}{\log d}.
$$

Consequently every such $F$ has

$$
D\geq\frac{h}{2d\log d}\left(\log\frac n2-1\right),
$$

which proves the [L1 distortion lower bound for an expander graph](../../../../../l1-distortion-lower-bound-for-an-expander-graph.md).

Finally, suppose an expander family admitted uniform coarse embeddings $F_n$ into $L^1$. Embedded edges have length at most $\rho_+(1)$, whereas the preceding Poincare argument and the fact that at least half the ordered pairs have distance comparable to $\log|V_n|$ imply

$$
d\rho_+(1)\geq\frac h2\rho_-(c\log|V_n|).
$$

This contradicts $\rho_-(t)\to\infty$. Thus expanders do not uniformly coarsely embed into $L^1$. They do not uniformly coarsely embed into $L^2$ either: a Hilbert space embeds isometrically into an $L^1$ space by

$$
v\longmapsto\left(\omega\mapsto
\frac{\langle v,g(\omega)\rangle}{\mathbb E|N(0,1)|}
\right),
$$

so an $L^2$ coarse embedding would produce an $L^1$ one. This is the [expander graph obstruction to uniform coarse embedding](../../../../../expander-graph-obstruction-to-uniform-coarse-embedding.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 155](../../paper-155-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
