<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Include the empty set, and take all unions of intervals $[a,b)$ with $a<b$. These intervals cover the real line, and the intersection of two is either empty or $[\max(a,c),\min(b,d))$. Distributing intersections over unions therefore makes finite intersections of open sets open; arbitrary unions are open by construction. The whole line is open, so the axioms of a [topology](../../../../../topology-split.md) hold. This is the [lower limit topology](../../../../../lower-limit-topology.md), whose space is the [Sorgenfrey line](../../../../../lower-limit-topology.md).

If $x<y$, the neighborhoods $[x,y)$ and $[y,y+1)$ are disjoint. Hence $\boxed{(\mathbb R,\tau_1)\text{ is Hausdorff}}$.

For the identity into the [cofinite topology](../../../../../cofinite-topology.md), an inverse image is the same subset of $\mathbb R$. Let $F$ be finite and $x\notin F$. If $F$ has a point greater than $x$, choose $b$ to be its least such point; otherwise take $b=x+1$. Then $[x,b)$ avoids every point of $F$, including $b$ itself. Taking these intervals over all $x\notin F$ writes $\mathbb R\setminus F$ as a $\tau_1$-open set. The inverse image of every cofinite open set, and of the empty set, is open. **The identity map is continuous**, because $\tau_2\subseteq\tau_1$.

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
