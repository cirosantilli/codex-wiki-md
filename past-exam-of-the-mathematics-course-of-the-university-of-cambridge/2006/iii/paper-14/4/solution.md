<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the unheaded degree-one continuation, write $X=\sum_{v=1}^n I_v$, where $I_v$ indicates that vertex $v$ has degree one. With

$$
q=\mathbb P(I_v=1)=(n-1)p(1-p)^{n-2},
$$

we have

$$
\mathbb E X=nq\sim e^{-c}(\log n+c)\longrightarrow\infty.
$$

For distinct vertices $u,v$, separate the cases where their connecting [edge](../../../../../edge-of-a-graph.md) is present or absent. If it is present, all their other incident [edges](../../../../../edge-of-a-graph.md) must be absent. If it is absent, each vertex chooses its unique neighbour among the other $n-2$ vertices; those two neighbours may coincide. The respective [edge](../../../../../edge-of-a-graph.md) constraints are [independent](../../../../../independent-random-variables.md) even in that case. Thus

$$
\mathbb E(I_uI_v)=p(1-p)^{2n-4}+(n-2)^2p^2(1-p)^{2n-5}.
$$

Dividing by $q^2$ gives the exact ratio

$$
R_n=\frac{1}{(n-1)^2p}+\left(\frac{n-2}{n-1}\right)^2\frac{1}{1-p}\longrightarrow1.
$$

The first term tends to zero because $(n-1)^2p$ has order $n\log n$; the second tends to one. Consequently its [variance](../../../../../variance-split.md) satisfies

$$
\frac{\operatorname{Var}X}{(\mathbb EX)^2}
=\frac{1}{nq}+\left(1-\frac1n\right)R_n-1\longrightarrow0.
$$

The [Chebyshev inequality](../../../../../chebyshev-inequality.md) now yields $\mathbb P(X=0)\leq\operatorname{Var}X/(\mathbb EX)^2\to0$. **A vertex of degree one exists [with high probability](../../../../../with-high-probability.md)**, even though the limiting [probability](../../../../../probability.md) of having an [isolated vertex](../../../../../isolated-vertex.md) is strictly between zero and one.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
