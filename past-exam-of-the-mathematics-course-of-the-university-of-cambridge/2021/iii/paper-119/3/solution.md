<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [cocone under a diagram](../../../../../cocone-under-a-diagram.md) $D:\mathcal J\to\mathcal C$ with vertex $X$ is a natural family $\lambda_j:Dj\to X$, so $\lambda_kD(u)=\lambda_j$ for every $u:j\to k$. A [colimit](../../../../../colimit.md) of $D$ is an initial such cocone: for every cocone $\lambda:D\Rightarrow\Delta X$, there is a unique $h:\operatorname{colim}D\to X$ with $h\iota_j=\lambda_j$ for all $j$.

Let $F:\mathcal I\to\mathcal J$ be a [final functor](../../../../../final-functor.md) and let $\lambda_i:D(Fi)\to X$ be a cocone under $DF$. For each $j$, choose an object $(i,u:j\to Fi)$ of the nonempty [comma category](../../../../../comma-category.md) $(j\downarrow F)$ and define

$$
\bar\lambda_j=\lambda_iD(u):D(j)\to X.
$$

A morphism $(i,u)\to(i',u')$ in the comma category gives $F(v)u=u'$, and the cocone identity shows that the two resulting maps are equal. Because $(j\downarrow F)$ is a [connected category](../../../../../connected-category.md), a zigzag proves independence of the chosen object. The same construction applied after a morphism $j\to k$ proves naturality, so $\bar\lambda$ is a cocone. Any extension must have this value because it must satisfy the cocone identity along $u$, proving uniqueness. This is [cocone extension along a final functor](../../../../../cocone-extension-along-a-final-functor.md).

If $L$ is a colimit of $DF$, its universal cocone extends uniquely to $D$. Restriction and extension give mutually inverse correspondences between cocones from $D$ and from $DF$, so the extended cocone is a colimit of $D$. Therefore the existence of all colimits of shape $\mathcal I$ implies the required colimits of shape $\mathcal J$.

Now suppose $\mathcal J$ is a [sifted category](../../../../../sifted-category.md). For $D,E:\mathcal J\to\mathbf{Set}$, the product functor $-\times A$ is a [left adjoint](../../../../../adjoint-functors.md), so it preserves colimits. Applying this once in each variable gives

$$
\left(\operatorname*{colim}_{j\in\mathcal J}D_j\right)
\times
\left(\operatorname*{colim}_{k\in\mathcal J}E_k\right)
\cong
\operatorname*{colim}_{(j,k)\in\mathcal J\times\mathcal J}(D_j\times E_k).
$$

The diagonal $\Delta:\mathcal J\to\mathcal J\times\mathcal J$ is final, so the right side is

$$
\operatorname*{colim}_{j\in\mathcal J}(D_j\times E_j).
$$

Thus $\operatorname{colim}_{\mathcal J}$ preserves binary [products in a category](../../../../../product-category-theory.md). Since $\mathcal J$ is connected, the colimit of the constant singleton diagram is a singleton, so it also preserves the [terminal object](../../../../../terminal-object.md). It therefore preserves finite products.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
