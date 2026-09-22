<h1 id="21g/solution">Solution</h1>

↑ **Parent:** [21G](../21g.md)

The real [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) says that if $X$ is compact Hausdorff and $A\subset C(X,\mathbb R)$ is a subalgebra containing the constants and separating points, then $A$ is uniformly dense in $C(X,\mathbb R)$.

Let $\overline A$ be the uniform closure. [Polynomial](../../../../../polynomial-split.md) approximation to $\sqrt t$ on a bounded interval shows that $|f|\in\overline A$ whenever $f\in\overline A$. Hence $\overline A$ is closed under

$$
\max(f,g)=\frac{f+g+|f-g|}{2},\qquad
\min(f,g)=\frac{f+g-|f-g|}{2}.
$$

Given $h\in C(X)$, separation and the constants provide, for each $x,y$, a [function](../../../../../function-split.md) in $A$ agreeing with $h$ at $x$ and $y$. Compactness first combines finitely many such [functions](../../../../../function-split.md) by minima to obtain one that agrees at $x$ and lies below $h+\varepsilon$ everywhere; a second finite cover and maxima produces $f\in\overline A$ with $|f-h|<\varepsilon$. Thus $h\in\overline A$.

The space $C_b(\mathbb R)$ is Banach because a uniform Cauchy [sequence](../../../../../sequence.md) converges uniformly to a bounded [continuous function](../../../../../continuous-function.md). Compactness is essential: the algebra of bounded [continuous functions](../../../../../continuous-function.md) having finite [limits](../../../../../limit-of-a-function.md) at both $+\infty$ and $-\infty$ contains constants and separates points, for example using $\tanh x$, but its uniform closure has the same limiting property. It cannot uniformly approximate $\sin x$, so it is not dense in $C_b(\mathbb R)$.

## ↑ Ancestors (10)

1. [21G](../21g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
