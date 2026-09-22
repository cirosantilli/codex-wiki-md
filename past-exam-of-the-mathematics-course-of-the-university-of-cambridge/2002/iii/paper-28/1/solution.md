<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In [bond percolation](../../../../../bond-percolation-split.md) on the [square lattice](../../../../../square-lattice.md), every nearest-neighbour [edge](../../../../../edge-of-a-graph.md) independently has state one, meaning open, with [probability](../../../../../probability.md) $p$, and state zero, meaning closed, with [probability](../../../../../probability.md) $1-p$. Thus the configuration law is the [product measure](../../../../../product-measure.md) $\mathbb P_p=\bigotimes_{e\in E}\operatorname{Bernoulli}(p)$. An [open path in bond percolation](../../../../../open-path-in-bond-percolation.md) uses only open [edges](../../../../../edge-of-a-graph.md). An [increasing event](../../../../../increasing-event.md) $A$ satisfies $\omega\in A,\ \omega'\ge\omega\Rightarrow\omega'\in A$: opening further [edges](../../../../../edge-of-a-graph.md) cannot destroy the event.

The [Harris-FKG inequality](../../../../../harris-fkg-inequality.md) for two increasing events is

$$
\boxed{\mathbb P_p(A\cap B)\ge\mathbb P_p(A)\mathbb P_p(B)}.
$$

For [disjoint occurrence of increasing events](../../../../../disjoint-occurrence-of-increasing-events.md), write $A\square B$ when disjoint sets of open [edges](../../../../../edge-of-a-graph.md) separately witness $A$ and $B$, so each event is forced by its own witness regardless of the other [edges](../../../../../edge-of-a-graph.md). The [Van den Berg-Kesten inequality](../../../../../van-den-berg-kesten-inequality.md) states

$$
\boxed{\mathbb P_p(A\square B)\le\mathbb P_p(A)\mathbb P_p(B)}.
$$

For events given by [cylinder sets](../../../../../cylinder-set.md) these are finite-coordinate assertions. Connection events have finite open-path witnesses; truncating to finite boxes and taking increasing limits gives the same disjoint-occurrence bound for them. Sharing a [vertex](../../../../../vertex-graph-theory.md) between the two witness paths is permitted; sharing an [edge](../../../../../edge-of-a-graph.md) is not.

For $1\le m<n$, take a simple open path from the origin to the radius-$n$ boundary and let $x$ be its first [vertex](../../../../../vertex-graph-theory.md) on the radius-$m$ boundary. Its initial segment witnesses $0\leftrightarrow x$. If $z$ is its final [vertex](../../../../../vertex-graph-theory.md), then $\|z-x\|_\infty\ge n-m$. Consequently the remaining segment reaches $x+\partial\Lambda_{n-m}$, and its initial portion until that visit witnesses $x\leftrightarrow x+\partial\Lambda_{n-m}$. The two segments use disjoint [edges](../../../../../edge-of-a-graph.md). Hence

$$
\{0\leftrightarrow\partial\Lambda_n\}
\subseteq\bigcup_{x\in\partial\Lambda_m}
\bigl(\{0\leftrightarrow x\}\square\{x\leftrightarrow x+\partial\Lambda_{n-m}\}\bigr).
$$

The [union bound](../../../../../boole-s-inequality.md), [Van den Berg-Kesten inequality](../../../../../van-den-berg-kesten-inequality.md) and [translation invariance](../../../../../translation-invariance.md) of the [product measure](../../../../../product-measure.md) now give the [weighted BK boundary-splitting estimate](../../../../../weighted-bk-boundary-splitting-estimate.md)

$$
\boxed{g_n\le g_{n-m}\sum_{x\in\partial\Lambda_m}\mathbb P_p(0\leftrightarrow x)}.
$$

For $m=n$ the same bound follows directly from the [union bound](../../../../../boole-s-inequality.md), with $g_0=1$. With the conventional $\partial\Lambda_0=\{0\}$, $m=0$ gives equality.

Write $C(0)$ for the [percolation cluster](../../../../../percolation-cluster.md) of the origin. By summing its membership indicators, the [percolation susceptibility](../../../../../percolation-susceptibility.md) is

$$
\chi(p)=\mathbb E_p|C(0)|=\sum_{x\in\mathbb Z^2}\mathbb P_p(0\leftrightarrow x)
=1+\sum_{m\ge1}a_m,\qquad
 a_m=\sum_{x\in\partial\Lambda_m}\mathbb P_p(0\leftrightarrow x).
$$

If it is finite, then $a_m\to0$. For $0<p<1$, choose $m$ with $0<a_m=a<1$. Iterating the boundary-splitting estimate with this fixed $m$ gives

$$
g_k\le a^{\lfloor k/m\rfloor}g_{k-m\lfloor k/m\rfloor}
\le a^{\lfloor k/m\rfloor}.
$$

For $k\ge2m$, $\lfloor k/m\rfloor\ge k/(2m)$, so $g_k\le\exp[-(-\log a)k/(2m)]$. To handle all smaller positive radii without an unspecified prefactor, observe that $g_k\le g_1=1-(1-p)^4<1$. Therefore

$$
\boxed{\gamma=\min\left\{\frac{-\log a}{2m},\frac{-\log g_1}{2m}\right\}>0,
\qquad g_k\le e^{-\gamma k}\quad(k\ge0)}.
$$

For $1\le k<2m$, the second chosen rate gives $e^{-\gamma k}\ge g_1$, and for larger $k$ the first rate applies. At $k=0$ both sides equal one. The endpoint $p=0$ has $g_k=0$ for every $k\ge1$, so any positive rate works; $p=1$ is excluded by finite susceptibility. This proves [exponential one-arm decay from finite susceptibility](../../../../../exponential-one-arm-decay-from-finite-susceptibility.md) with the required unit prefactor.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
