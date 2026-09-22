<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $u:X\to U_{\mathcal K}$ be continuous. The family $\{u(x)-I:x\in X\}$ is norm compact in the compact-operator ideal. For any $\varepsilon>0$ there is one finite-rank [orthogonal projection](../../../../../../orthogonal-projection.md) $P$ with

$$
\sup_x\|u(x)-I-P(u(x)-I)P\|<\varepsilon.
$$

To prove it, take a finite $\varepsilon$-net of [compact operators](../../../../../../compact-operator-split.md), approximate each by a [finite-rank operator](../../../../../../finite-rank-operator.md), and include both their ranges and adjoint ranges in $P\mathcal H$. Contractivity of compression transfers the estimate to the whole family.

Take $\varepsilon<1$ and set $g(x)=I+P(u(x)-I)P$. It is invertible because it is within distance one of the unitary $u(x)$. It has the form $g_V(x)\oplus I$ on $V\oplus V^\perp$, where $V=P\mathcal H$ is finite-dimensional and $g_V:X\to GL(V)$ is continuous. The straight segment from $u$ to $g$ stays invertible; taking its unitary polar factors supplies a [homotopy](../../../../../../homotopy.md) in $U_{\mathcal K}$, since inverse square root depends continuously on the positive invertible factors and preserves identity modulo compacts.

Conversely a map $g:X\to GL(V)$ defines such a class by the continuous deformation $g(g^*g)^{-t/2}$ to its unitary polar factor, then extension by the identity on $V^\perp$. Apply the same uniform finite-rank approximation to a [homotopy](../../../../../../homotopy.md) on the compact space $X\times[0,1]$. Choosing $P$ to include the original endpoint supports keeps those endpoints unchanged under compression. This proves that two finite-dimensional maps give the same class exactly when, after adding identity blocks, they are homotopic through a common finite-dimensional [general linear group](../../../../../../general-linear-group.md). Hence

$$
\boxed{K^1(X)=\underset{N}{\operatorname{colim}}\,[X,GL_N(\mathbb C)],}
$$

with stabilization $g\mapsto\operatorname{diag}(g,1)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
