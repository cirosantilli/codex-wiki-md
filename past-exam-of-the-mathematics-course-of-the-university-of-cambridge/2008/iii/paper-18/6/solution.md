<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A real rank-$d$ [vector bundle](../../../../../vector-bundle.md) $p:E\to M$ is a continuous family of $d$-dimensional real vector spaces, locally trivial by homeomorphisms $p^{-1}(U)\cong U\times\mathbb R^d$ which are linear on every fiber. Transition matrices are continuous maps into $\operatorname{GL}_d(\mathbb R)$. The [Grassmannian](../../../../../grassmannian.md) $\operatorname{Gr}_k(\mathbb R^n)$ is the space of $k$-dimensional linear subspaces; its topology can be defined by identifying each plane $W$ with its orthogonal projection matrix $P_W$. Local graph charts identify nearby planes with graphs of maps $W_0\to W_0^\perp$.

The [tautological bundle](../../../../../tautological-bundle.md) is $E_{\rm taut}=\{(W,v):v\in W\}\to\operatorname{Gr}_k(\mathbb R^n)$. In graph charts a basis of $W_0$ gives a continuously varying basis of each graph, proving local triviality. The [universal quotient bundle](../../../../../universal-quotient-bundle-on-a-real-grassmannian.md) has fiber $Q_W=\mathbb R^n/W$. The map $[v]\mapsto(I-P_W)v$ identifies it continuously with the orthogonal-complement bundle $W^\perp$, whose graph charts similarly supply local frames. Thus $Q_{\rm taut}$ is a rank-$(n-k)$ [quotient vector bundle](../../../../../quotient-vector-bundle.md).

For the given $E\to M$, at each $m$ choose a basis of $E_m$ and global [sections of a vector bundle](../../../../../section-of-a-vector-bundle.md) realizing its basis vectors, using the evaluation-surjectivity assumption. Those $d$ sections remain independent on a neighbourhood of $m$, since the corresponding determinant in a local trivialization is nonzero at $m$ and continuous. Compactness gives a finite cover by such neighbourhoods. Collect all the selected sections as $s_1,\ldots,s_N$; they span every fiber. They define a fiberwise surjective [vector bundle morphism](../../../../../vector-bundle-morphism.md)

$$
F:M\times\mathbb R^N\longrightarrow E,\qquad F_m(c_1,\ldots,c_N)=\sum_{j=1}^N c_js_j(m).
$$

Its kernels have constant dimension $N-d$ and form the [kernel bundle of a surjective vector bundle morphism](../../../../../kernel-bundle-of-a-surjective-vector-bundle-morphism.md). More concretely, in a local frame of $E$ the map has a continuous full-row-rank matrix $A(m)$ and its kernel projection is

$$
P_{\ker F_m}=I_N-A(m)^T\bigl(A(m)A(m)^T\bigr)^{-1}A(m).
$$

This varies continuously and is unchanged by an invertible change of target frame. The [Grassmannian as projection matrices](../../../../../grassmannian-as-projection-matrices.md) therefore makes

$$
\phi(m)=\ker F_m\in\operatorname{Gr}_{N-d}(\mathbb R^N)
$$

a continuous map. The fiber quotient map induced by $F_m$ is an isomorphism $\mathbb R^N/\ker F_m\to E_m$. The same local matrix formula gives continuously varying right inverses, so these fiber isomorphisms give a [vector bundle isomorphism](../../../../../vector-bundle-isomorphism.md). This proves the [classification of vector bundles by a universal quotient bundle](../../../../../classification-of-vector-bundles-by-a-universal-quotient-bundle.md):

$$
\boxed{E\cong\phi^*Q_{\rm taut}.}
$$

The displayed equality in the classification statement is understood as bundle isomorphism, not literal equality of total spaces.

Finally, the [universal quotient bundle need not have a nowhere-zero section](../../../../../universal-quotient-bundle-need-not-have-a-nowhere-zero-section.md). Take $\operatorname{Gr}_1(\mathbb R^2)=\mathbb{RP}^1$. Its quotient identifies with $W^\perp$, a [Möbius line bundle](../../../../../mobius-line-bundle.md). Write $W_\theta=\operatorname{span}(\cos\theta,\sin\theta)$, with $\theta$ modulo $\pi$. A section of the complement line has the form $a(\theta)(-\sin\theta,\cos\theta)$, and being single-valued requires $a(\theta+\pi)=-a(\theta)$. If $a$ is nonzero anywhere, the intermediate value theorem forces a zero between that point and its translate by $\pi$; if it is nowhere nonzero the conclusion is immediate. Hence **this rank-one quotient bundle has no nowhere-zero section**.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
