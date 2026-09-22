<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here a [pointed complete partial order](../../../../../../pointed-complete-partial-order.md) is a [partially ordered set](../../../../../../partially-ordered-set.md) $D$ with a least element $\bot_D$ in which every nonempty [directed set](../../../../../../directed-set.md) has a [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md). Directed means that every pair of its elements has an upper bound within that set. A [Scott continuous map](../../../../../../scott-continuous-map.md) is monotone and preserves these directed suprema. It is not required to preserve the least element; restricting to strict maps would change the categorical claim. If completeness is instead formulated only for increasing countable chains, the same arguments below work with those chains.

Order the [function space of complete partial orders](../../../../../../function-space-of-complete-partial-orders.md) $[D\to E]$ pointwise: $f\leq g$ means $f(x)\leq g(x)$ for every $x$. Its least element is the constant function with value $\bot_E$. For a directed family $\mathcal F$ of continuous maps, define $h(x)=\sup_{f\in\mathcal F}f(x)$. This is well-defined and is its pointwise [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md). It is monotone. For any directed $A\subseteq D$,

$$
h(\sup A)=\sup_f f(\sup A)=\sup_f\sup_{a\in A}f(a)=\sup_{a\in A}\sup_f f(a)=\sup h[A].
$$

The interchange is valid because the combined family $\{f(a):f\in\mathcal F,a\in A\}$ is directed, and either iterated supremum is its [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md). Thus $h$ is a [Scott continuous map](../../../../../../scott-continuous-map.md), proving that **$[D\to E]$ is a [pointed complete partial order](../../../../../../pointed-complete-partial-order.md)**.

Finite products carry the [product order](../../../../../../product-order.md), componentwise suprema and least element $(\bot_D,\bot_E)$. The one-element order is a [terminal object](../../../../../../terminal-object.md). For the exponential, use the function space with evaluation $\operatorname{ev}(f,x)=f(x)$. To check joint continuity, take a directed family of pairs $(f_i,x_i)$. Then

$$
\operatorname{ev}(\sup_i f_i,\sup_i x_i)=\sup_i\sup_j f_i(x_j)=\sup_k f_k(x_k).
$$

Indeed, directedness supplies a $k$ above the pairs indexed by both $i$ and $j$, giving $f_i(x_j)\leq f_k(x_k)$. Thus the diagonal values are cofinal in the double family, and evaluation preserves its supremum.

For a continuous $h:A\times D\to E$, its [currying](../../../../../../currying.md) is $\Lambda h:A\to[D\to E]$, $(\Lambda h)(a)(d)=h(a,d)$. Each section is continuous because $d\mapsto(a,d)$ is; pointwise directed suprema in the $a$ coordinate show that $\Lambda h$ is continuous. Conversely a continuous $g:A\to[D\to E]$ gives the continuous map $\operatorname{ev}\circ(g\times\operatorname{id}_D)$. The two constructions are inverse, because they agree on every pair $(a,d)$. This gives the natural bijection

$$
\boxed{\operatorname{Hom}(A\times D,E)\cong\operatorname{Hom}(A,[D\to E]),}
$$

with the required evaluation map. Together with the [terminal object](../../../../../../terminal-object.md) and products, it proves **cartesian closure of pointed complete partial orders with non-strict continuous maps**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
