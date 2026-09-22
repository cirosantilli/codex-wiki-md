<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $B_n=\phi(0\leftrightarrow\partial\Lambda_n)$ and $s_n=|\partial\Lambda_n|$. This connection event is the union over $x\in\partial\Lambda_n$ of $\{0\leftrightarrow x\}$. The [union bound](../../../../../../boole-s-inequality.md) therefore supplies a [graph vertex](../../../../../../vertex-graph-theory.md) with connection [probability](../../../../../../probability.md) at least $B_n/s_n$.

Every boundary [graph vertex](../../../../../../vertex-graph-theory.md) has some coordinate equal to $n$ or $-n$. By applying a [permutation](../../../../../../permutation.md) and a [graph automorphisms](../../../../../../graph-automorphism.md), which preserve both the law and the boundary, choose such a [graph vertex](../../../../../../vertex-graph-theory.md) in the form $x=(n,x_2,\ldots,x_d)$ while retaining its [probability](../../../../../../probability.md) bound. Now $e_{2n}-x=(n,-x_2,\ldots,-x_d)$ is a reflection of $x$. Translation and reflection invariance give

$$
\phi(x\leftrightarrow e_{2n})=\phi(0\leftrightarrow e_{2n}-x)=\phi(0\leftrightarrow x).
$$

[Positive association of random variables](../../../../../../positive-association-of-random-variables.md) applied to the two connection events, whose intersection implies $0\leftrightarrow e_{2n}$, proves the [reflection comparison of random-cluster connections](../../../../../../reflection-comparison-of-random-cluster-connections.md):

$$
\boxed{C_{2n}\ge\phi(0\leftrightarrow x)^2,\qquad
\phi(0\leftrightarrow x)\ge B_n/s_n.}
$$

Also $C_n\le B_n$, since any path to $e_n$ meets the box boundary. Consequently

$$
C_n\le B_n\le s_n\sqrt{C_{2n}},
$$

and hence

$$
-\frac1{2n}\log C_{2n}-\frac{\log s_n}{n}
\le-\frac1n\log B_n
\le-\frac1n\log C_n.
$$

Here $s_n=(2n+1)^d-(2n-1)^d=O(n^{d-1})$, so $\log s_n/n\to0$. Both outside logarithmic connection rates converge to $\alpha(p,q)$ by part (b). Squeezing gives the rate for every box size, and therefore for the requested even subsequence:

$$
\boxed{-\frac1{2n}\log\phi^1_{p,q}(0\leftrightarrow\partial\Lambda_{2n})\longrightarrow\alpha(p,q).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
