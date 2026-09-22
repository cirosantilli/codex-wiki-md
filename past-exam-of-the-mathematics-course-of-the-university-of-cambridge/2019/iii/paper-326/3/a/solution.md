<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $u\in L^1(\Omega)$, the [total variation seminorm on a domain](../../../../../../total-variation-seminorm-on-a-domain.md) is

$$
\operatorname{TV}(u)=\sup_{\substack{\varphi\in C_c^\infty(\Omega;\mathbb R^n)\\\|\varphi\|_\infty\leq1}}
\int_\Omega u\,\operatorname{div}\varphi\,dx.
$$

Using $C_c^1$ instead gives the same definition. The zero test field shows nonnegativity, and $\operatorname{TV}(0)=0$, so this is a [proper extended-real function](../../../../../../proper-extended-real-function.md). Each test field defines a linear functional of $u$; taking their supremum proves [convexity](../../../../../../convex-function.md), equivalently

$$
\operatorname{TV}(tu+(1-t)v)\leq t\operatorname{TV}(u)+(1-t)\operatorname{TV}(v),\qquad0\leq t\leq1.
$$

It is **not strictly convex**: two distinct constant functions both have zero total variation, as does every convex combination of them.

The [function of bounded variation on a domain](../../../../../../function-of-bounded-variation-on-a-domain.md) space is

$$
BV(\Omega)=\{u\in L^1(\Omega):\operatorname{TV}(u)<\infty\},\qquad
\|u\|_{BV}=\|u\|_{L^1}+\operatorname{TV}(u).
$$

Total variation is **not coercive on $BV(\Omega)$**: for $u_k\equiv k$ on a domain of positive measure, $\|u_k\|_{BV}=k|\Omega|\to\infty$, whereas $\operatorname{TV}(u_k)=0$. This is [noncoercivity of total variation on constants](../../../../../../noncoercivity-of-total-variation-on-constants.md); a mean-zero constraint can remove the constant obstruction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
