<h1 id="3/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

By the definition of the [subdifferential](../../../../../../subdifferential.md), $p\in\partial J(u)$ means

$$
J(v)\geq J(u)+\langle v-u,p\rangle\quad\text{for every }v.
$$

Rearrangement bounds $\langle v,p\rangle-J(v)$ by $\langle u,p\rangle-J(u)$, and equality is attained at $v=u$. Taking the supremum in the definition of the [convex conjugate](../../../../../../convex-conjugate.md) gives $J^*(p)=\langle u,p\rangle-J(u)$. Conversely this equality bounds every member of that supremum and rearranges to the [subgradient](../../../../../../subgradient.md) inequality. Therefore

$$
\boxed{p\in\partial J(u)\iff J(u)+J^*(p)=\langle u,p\rangle.}
$$

Apply the same argument to $J^*$ and use the [Fenchel-Moreau theorem](../../../../../../fenchel-moreau-theorem.md) $J^{**}=J$. With the canonical Hilbert identification of the bidual, the equality is also equivalent to $u\in\partial J^*(p)$. This proves [subgradient inversion under convex conjugacy](../../../../../../subgradient-inversion-under-convex-conjugacy.md):

$$
\boxed{p\in\partial J(u)\iff u\in\partial J^*(p).}
$$

The conditions include finiteness at the points in question; expressions involving $+\infty$ are not [subgradients](../../../../../../subgradient.md) merely by formal subtraction.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
