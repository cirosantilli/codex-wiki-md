# Least fixed point from a directed family of maps

↑ **Parent:** [Directed-complete partial order](directed-complete-partial-order.md)

Let $f$ be [order-preserving](order-preserving-function.md) and [inflationary](inflationary-map.md) on a [directed-complete partial order](directed-complete-partial-order.md). Define $x\mathrel R y$ when every set containing $x$ and closed under $f$ and directed [joins](least-upper-bound-in-a-partially-ordered-set.md) contains $y$. This is a [partial order](partially-ordered-set.md) refining $\le$. The [order-preserving](order-preserving-function.md) maps $h$ satisfying $x\mathrel R h(x)$ form a composition-closed family $H$. The values $H x$ are [directed](directed-set.md), since $h(k(x))$ bounds $h(x)$ and $k(x)$. Their [least upper bound](least-upper-bound-in-a-partially-ordered-set.md) $h_0(x)$ lies in every such closed set containing $x$, so $h_0\in H$. Then $f\circ h_0\in H$ gives $f(h_0(x))\le h_0(x)$, while inflationarity gives the reverse inequality. If $p=f(p)$ and $x\le p$, the lower set $\{y:y\le p\}$ is closed, proving $h_0(x)\le p$. Thus $h_0(x)$ is the least [fixed point](fixed-point.md) of $f$ above $x$.

## ↑ Ancestors (9)

1. [Directed-complete partial order](directed-complete-partial-order.md)
2. [Complete partial order](complete-partial-order.md)
3. [Partially ordered set](partially-ordered-set.md)
4. [Set](set-split.md)
5. [Set theory](set-theory-split.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/16g/solution.md)
