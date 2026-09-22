<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take a locally finite trivializing cover $(U_\alpha)$ of the real [vector bundle](../../../../../vector-bundle.md) $E$, and a subordinate smooth [partition of unity](../../../../../partition-of-unity.md) $(\rho_\alpha)$. Each trivialization identifies its fibers with $\mathbb R^m$ and hence supplies a smooth Euclidean [inner product](../../../../../inner-product.md) $g_\alpha$ there. Define

$$
\boxed{g_b(v,w)=\sum_\alpha\rho_\alpha(b)(g_\alpha)_b(v,w).}
$$

Each weighted term extends by zero outside its chart, since the weight has support within that chart. Local finiteness makes the sum smooth in every bundle chart. At each $b$ at least one weight is positive; for $v\ne0$ every nonzero contribution to $g_b(v,v)$ is positive. Thus $g$ is a smooth positive-definite [fiber metric](../../../../../fiber-metric.md), which is precisely an inner product varying smoothly with the fibers.

A [G-structure on a vector bundle](../../../../../g-structure-on-a-vector-bundle.md) is a reduction of its [frame bundle](../../../../../frame-bundle.md) from $GL(m,\mathbb R)$ to $G$: a principal $G$-subbundle $P\subseteq\operatorname{Fr}(E)$ whose extension of structure group is the full frame bundle. Equivalently, it is a choice of smooth local frames with transition matrices in $G$, and the reduction consists of the right $G$-orbits of these frames. The adapted frames are part of the structure, not merely a statement that an individual fiber has a basis.

Given a [fiber metric](../../../../../fiber-metric.md), the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) transforms any smooth local frame into [Euclidean orthonormal frames](../../../../../euclidean-orthonormal-frame.md). At each step the squared norm to be divided out is positive, so the divisions and positive square roots depend smoothly on the base point. Two such frames differ by an orthogonal matrix. All the orthonormal frames therefore form a principal $O(m)$ reduction, an [orthogonal structure on a real vector bundle](../../../../../orthogonal-structure-on-a-real-vector-bundle.md).

Conversely, let $P$ be an $O(m)$ reduction. A frame $u:\mathbb R^m\to E_b$ in $P_b$ defines

$$
g_b(ua,uc)=a\cdot c.
$$

Replacing $u$ by $uq$ for $q\in O(m)$ leaves this rule unchanged, since $q$ preserves the Euclidean inner product. It is consequently independent of the adapted frame and defines a positive-definite [fiber metric](../../../../../fiber-metric.md). Its coefficients are smooth in local adapted frames. These constructions are mutually inverse. **An $O(m)$-structure is equivalent to a smooth fiberwise inner product.**

For $SO(m)$, the additional condition is an [orientation of a vector bundle](../../../../../orientation-of-a-vector-bundle.md). Such a reduction supplies consistently oriented orthonormal frames, since its transition determinants are $+1$. Conversely an orientation together with a [fiber metric](../../../../../fiber-metric.md) selects the oriented Euclidean orthonormal frames and gives an $SO(m)$ reduction. Thus

$$
\boxed{E\text{ admits an }SO(m)\text{-structure}\iff E\text{ is orientable}.}
$$

It is not true for every real bundle. The [Möbius line bundle](../../../../../mobius-line-bundle.md) is obtained from $[0,2\pi]\times\mathbb R$ by $(2\pi,v)\sim(0,-v)$. If it had an orientation, hence a nowhere-zero continuous section, its coefficient on the interval would satisfy $f(2\pi)=-f(0)$ while staying nonzero. The intermediate value theorem makes that impossible. Since $SO(1)=\{1\}$, it has no $SO(1)$ reduction. For each $m\ge1$, its direct sum with a trivial rank-$(m-1)$ bundle has transition matrix $\operatorname{diag}(-1,1,\ldots,1)$ and determinant line equal to the Möbius line. It is also nonorientable and has no $SO(m)$-structure. This obstruction concerns the bundle's orientation, independently of the existence of a metric.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
